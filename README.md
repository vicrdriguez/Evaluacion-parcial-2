# Descripcion del proyecto 

Desarrollo de una arquitectura para una empresa que busca modernizarse con el formato industria 4.0 implementando un modelo de ia que sea posible de procesar datos agilmente y con la finalidad de visualizar dashboard para sus empleados sobre el procesod e datos de temperaturas y vibraciones para la planta de manefactura 

# Arquitectura seleccionada

la arquitectura que fue seleccionada es la Lakehouse ya que se necesitan recolectar datos de temperatura y vibración  donde sus datos son fijos y sin implementación de cambios haciendo que no sea necesario tener grandes bases de datos para guardar toda esta información siendo posible una escalabilidad simple gracias a sus datos no estructurados. En cuanto seguridad, es útil tener la seguridad separada por lógica ya que se usará el patrón capa medallion donde consiste en que cada capa tendrá su seguridad separada por roles asignados para controlar el acceso.Por último en la interoperabilidad lakehouse tiene un entorno unificado donde se pueden implementar herramientas sin la necesidad de mover servicios esto reduce mucho los costos y para el caso no se necesita tanta implementación.

# Requisitos y configuracion del entorno tecnico
# Herramientas utlizadas

Lenguaje de programacon utilizado: Python 
Almacenamiento de datos (base de datos): PostgreSQL
Control de versiones: Git y github
Contenedor de software: Docker


# Instruccion de instalacion


