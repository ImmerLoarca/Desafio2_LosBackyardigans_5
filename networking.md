##Solución para la Configuración de Red 

##Problema: Limitaciones del modo NAT en VirtualBox
Aunque permite acceso a Internet, aísla demasiado las máquinas virtuales. Esto impide que se comuniquen fácilmente entre ellas o con otros equipos de la red, lo que dificulta el trabajo en equipo.

##Diferencias: Las diferencias entre NAT, Adaptador puente y Red interna 

- NAT: Permite que la máquina virtual navegue en Internet
a través de la conexión del host. Sin embargo, otras máquinas de la red no pueden conectarse a ella, lo que la vuelve limitada para trabajo colaborativo.
- Puente (Bridge): Conecta la VM directamente a la red física, dándole una IP propia dentro del mismo rango que el resto de dispositivos. Así puede comunicarse con el host, otras VMs y equipos de la red sin restricciones.
- Red Interna: Crea una red privada solo entre VMs dentro de VirtualBox. Es útil para pruebas aisladas, pero no ofrece conexión al host ni a Internet.

##Propuesta: Para un entorno de desarrollo colaborativo, el modo Puente (Bridge Adapter) es el más adecuado ya que:
-Permite que todas las máquinas (VMs y PCs reales de la red) se vean entre sí.
-Facilita trabajar con servicios compartidos (ejemplo: una MV con servidor de base de datos, otra con API, otra con frontend).
Y así se simula mejor un entorno corporativo real.

##Como se configuraría 
Configurar una IP fija en Ubuntu es como darle a tu computadora un número de casa que nunca cambia. Normalmente el router asigna direcciones automáticamente, pero aquí elegimos un número específico (la IP) para que siempre sea el mismo. Además, le indicamos cuál es el router para salir a Internet (puerta de enlace) y qué servidores usar para traducir nombres de páginas web a direcciones que la computadora entiende (DNS). Así, la máquina siempre tendrá la misma dirección en la red, podrá comunicarse con otros equipos fácilmente y acceder a Internet de manera confiable

Autor: Javier Stanley Escobar Portillo

