# Solución para el Almacenamiento 

## Problema
Los fallos de disco en el servidor de archivos principal son críticos para la continuidad del negocio porque resultan en pérdida de datos irrecuperables, lo que puede interrumpir operaciones diarias, como el acceso a archivos compartidos, bases de datos de clientes o registros financieros. Esto genera downtime prolongado, afectando la productividad, la confianza de los clientes y potencialmente causando pérdidas económicas significativas. Sin redundancia, un solo fallo puede escalar a una crisis, violando principios de disponibilidad y resiliencia en entornos empresariales en crecimiento como TechSolutions Inc.

## Propuesta
Proponemos implementar RAID 5, que ofrece un equilibrio óptimo entre redundancia, capacidad de almacenamiento y rendimiento para un servidor de archivos. RAID 5 utiliza striping con paridad distribuida across al menos tres discos: los datos se dividen en bloques y se escribe paridad en uno de los discos por stripe. Esto permite tolerar la falla de un disco completo sin pérdida de datos, ya que la paridad permite reconstruir la información perdida.

## Justificación de la elección
A diferencia de RAID 1 (mirroring, que duplica datos pero desperdicia 50% de capacidad), RAID 5 maximiza el uso de espacio (capacidad efectiva = (n-1) * tamaño de disco, donde n es el número de discos) mientras proporciona redundancia. Comparado con RAID 10 (striping sobre mirrors), que requiere más discos y es más costoso, RAID 5 es eficiente para lecturas intensivas en servidores de archivos. Soluciona la redundancia al asegurar que los datos sigan accesibles durante un fallo, permitiendo hot-swapping de discos para minimizar downtime.

## Ejemplo de configuración en Linux (usando mdadm para software RAID):

Instalar mdadm: sudo apt install mdadm
Crear el array RAID 5 con 3 discos (/dev/sdb, /dev/sdc, /dev/sdd): sudo mdadm --create --verbose /dev/md0 --level=5 --raid-devices=3 /dev/sdb /dev/sdc /dev/sdd
Formatear y montar: sudo mkfs.ext4 /dev/md0 y sudo mount /dev/md0 /mnt/storage
Guardar configuración: sudo mdadm --detail --scan >> /etc/mdadm/mdadm.conf
 
Autor: Bryan Josue Diaz Ascencio
