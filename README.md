# Descripcion del proyecto 

Desarrollo de una arquitectura para una empresa que busca modernizarse con el formato industria 4.0 implementando un modelo de ia que sea posible de procesar datos agilmente y con la finalidad de visualizar dashboard para sus empleados sobre el procesod e datos de temperaturas y vibraciones para la planta de manefactura 

# Arquitectura seleccionada

la arquitectura que fue seleccionada es la Lakehouse ya que se necesitan recolectar datos de temperatura y vibración  donde sus datos son fijos y sin implementación de cambios haciendo que no sea necesario tener grandes bases de datos para guardar toda esta información siendo posible una escalabilidad simple gracias a sus datos no estructurados. En cuanto seguridad, es útil tener la seguridad separada por lógica ya que se usará el patrón capa medallion donde consiste en que cada capa tendrá su seguridad separada por roles asignados para controlar el acceso.Por último en la interoperabilidad lakehouse tiene un entorno unificado donde se pueden implementar herramientas sin la necesidad de mover servicios esto reduce mucho los costos y para el caso no se necesita tanta implementación.

# Requisitos y configuracion del entorno tecnico , Herramientas utlizadas

Lenguaje de programacon utilizado: Python 

Almacenamiento de datos (base de datos): PostgreSQL

Control de versiones: Git y github

Contenedor de software: Docker


# Instruccion de instalacion

 **Clonar el repositorio:**
    ```bash
    git clone https://github.com/usuario/proyecto.git
    ```
2.  **Instalar dependencias:**
    ```bash
    npm install  # O pip install -r requirements.txt

3. 
  **Levantamos los servicios de almacenamiento y procesamiento:**
    ```
    docker-compose up -d storage-engine spark-master

4.# Crear y activar entorno virtual
python -m venv venv
# En Windows: venv\Scripts\activate

5.
# Instalar dependencias de IA y Visualización
pip install -r requirements-analytics.txt





# Estructura del repositorio 

/
├── .github/workflows/         
├── config/                     
│   ├── infrastructure.yaml    
│   └── ml_params.yaml          
├── data/                      
│   ├── 01_bronze/             
│   ├── 02_silver/             
│   └── 03_gold/               
├── docs/                      
├── src/                        
│   ├── ingestion/              
│   │   ├── connectors/        
│   │   └── schema_validator.py 
│   ├── analytics/              
│   │   ├── features/           
│   │   ├── models/           
│   │   └── notebooks/          
│   └── ui/                     
├── tests/                     
├── docker-compose.yml          
├── requirements.txt            
└── README.md
