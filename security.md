# Implementacion de UFW

## Problema:
 Identifiquen las principales vulnerabilidades de seguridad que presenta la red
actual de TechSolutions Inc.

## Solucion por Equipo 5 - LosBackyardigans
Implementación de UFW con configuración de puertos y redes en especifico 

## Explicacion
Para la solución del problema implementaremos un sistema de seguridad que controlara las conexiones que entran y salen a su red bloqueando todo lo no deseado siendo como un filtro de lo que quiera que pase a su red y lo que no se quede fuera.

también se le harán cambios para permitir solo el acceso a SSH desde direcciones IP especificas esto se implementara configurando el sistema de seguridad antes mencionado para que permita el trafico de datos del puerto 22 que le pertenece a SSH, ya que se necesita bloquear los otros servicios pues eliminaremos de los servicios permitidos todos los que no terminen en puerto 22 y para las red especifica solo pondremos la red especifica y de la cual queremos recibir conexión y que pertenezca al puerto 22 antes mencionado para solo recibir conexión de esa red especifica y del servicio en especifico que seria el SSH por lo tanto se puede administrar su servidor remotamente.

# Autor: Diego Osorio.




