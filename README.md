# Proyecto Individual N° 2: Data Analyst (DA)

Resolución del segundo proyecto individual del BootCamp Data Science (dataft21) de Soy Henry

## Introducción

En Buenos Aires, los accidentes de tráfico son una preocupación diaria que involucra a todos los usuarios de la vía, con consecuencias que van desde daños materiales hasta lesiones mortales. La densidad de tráfico y poblacional exacerba el riesgo, impactando la seguridad pública y la infraestructura. Las tasas de mortalidad por accidentes viales, un indicador clave de la seguridad vial, reflejan la urgencia de reducir estos incidentes para salvar vidas. Anualmente, los siniestros viales son la principal causa de muertes violentas en Argentina, con aproximadamente 4,000 fallecimientos y una tendencia que supera las muertes por delitos.

Este proyecto tiene como objetivo principal analizar la información relacionada con los fallecimientos en accidentes de tráfico en Buenos Aires durante el periodo 2016-2021. La finalidad es producir datos y conclusiones relevantes que sirvan a las autoridades para establecer estrategias que reduzcan eficientemente el número de muertes y lesionados en dichos incidentes.

## Metodología y herramientas

El proyecto se desarrolló siguiendo estos pasos:

1. **Recopilación de Datos**: Se recolectaron datos de la Secretaría de Transporte de Buenos Aires, que incluían detalles sobre lesiones y homicidios en accidentes viales.

2. **Limpieza y preprocesamiento de Datos (ETL)**: Se organizó y limpió la información utilizando herramientas como Numpy y Pandas.

3. **Análisis Exploratorio de Datos (EDA)**: Se realizó un análisis preliminar para identificar patrones y obtener insights sobre los homicidios en accidentes de tráfico.

4. **Revisión del progreso de los objetivos estratégicos (KPI)**: Se analizó los resultados de 3 indicadores de progreso sobre objetivos estratégicos previamente decididos

Se utilizó las siguientes herramientas (Stack tecnológico):

![Static Badge](https://img.shields.io/badge/Python-gray?style=flat&logo=python) ![Static Badge](https://img.shields.io/badge/-Pandas-gray?style=flat&logo=pandas) ![Static Badge](https://img.shields.io/badge/Numpy-gray?style=flat&logo=numpy) ![Static Badge](https://img.shields.io/badge/-Matplotlib-gray?style=flat&logo=matplotlib) ![Static Badge](https://img.shields.io/badge/-Seaborn-gray?style=flat&logo=seaborn) ![Static Badge](https://img.shields.io/badge/PowerBI-gray?style=flat&logo=powerbi)


## Estructura del repositorio

- Carpeta Datasets: Donde se encuentran los archivos originales sin modificación que se usaron en el proyecto.
- Carpeta Notebooks: Donde se encuentran los notebooks de trabajo preliminar de ETL, EDA y KPis.
- Archivo .gitigonre: Archivo para establecer las carpetas y archivos que no serán revisados por el sistema Git
- Archivo Notas.md: Simples notas del autor
- Archivo README.md: Este archivo
- DashBoard .pbi:x  Archivo Power BI con un tablero resumen interactivo de todo lo hayado en el proyecto _______________________________________________________________________

## Desarrollo

En el proyecto se utilizó la **Base de Datos de Víctimas Fatales en Accidentes de Tráfico**, en el que se usaros los datasets de homicidios y lesiones (archivos de Excel) con dos secciones principales:

- **HECHOS**: Incluye un registro por cada evento con un identificador único y datos sobre el tiempo, lugar e involucrados.

- **VÍCTIMAS**: Presenta un registro por cada persona afectada, detallando su edad, género y medio de transporte, y se relaciona con los HECHOS a través del identificador del evento.


En el [documento](Orig/NOTAS_HOMICIDIOS_SINIESTRO_VIAL.pdf) se explican las definiciones usadas en los datos y en el proyecto. Además, los datos empleados están disponibles en este [enlace](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales).

Para el **Proceso de ETL (Extracción, Transformación y Carga)**, se extrajeron y limpiaron los datos de los conjuntos `HECHOS` y `VÍCTIMAS` usando Numpy y Pandas en Notebooks de Visual Studio Code. Se eliminaron valores nulos y duplicados, se realizaron cambios en los tipos de datos, se descartaron columnas innecesarias y se combinaron las tablas en un solo archivo [siniestros_limpio.csv](Datasets/siniestros.csv). Revisar código ETL en [01_ETL.ipynb](Notebooks/01_ETL.ipynb)

Durante el **Proceso de EDA (Análisis Exploratorio de Datos)**, se analizaron las relaciones entre las variables numéricas y categóricas de los conjuntos de datos limpios, se identificaron posibles anomalías y se buscaron patrones útiles para análisis futuros. Revisar código EDA en [02_EDA.ipynb](Notebooks/02_EDA.ipynb)

Luego el **Proceso de KPI (Indicador Clave de Desempeño)**, que sigue del Análisis Exploratorio de Datos, se utiliza los dataset resultantes [homicidios_limpio.csv](Datasets/homicidios_limpio.csv), [lesiones_limpio.csv](Datasets/lesiones_limpio.csv) y las comunas extraídas de fuente de terceros [Comunas](Notebooks/mapa_comunas.csv)  inicialmente en un Notebook [03_KPIs.ipynb](Notebooks/03_KPIs.ipynb) para finalmente presentarlos mediante en Dashboard de Power BI. La separación es que en los Notebooks de Python es más facil experimentar para encontrar insights y en los dashboard de Power Bi para moestrar lo encontrado, aunque ambas herramientas se podrían utilizar para analizar y mostrar.

Desarrollo (ETL, EDA y KPI y textos)

Conclusiones

