# Resumen de lo pedido
- Notebooks > Readme.md > Dashboard > Repositorio
- Readme.md: Detalle de archivos y carpetas del  repositorio. Reporte de análisis en base a dashboards
- ¿Mapas? con data de cámaras y comunas
- Archivo enviroment

# Comandos
- conda create --name PI2 python==3.11 ipykernel numpy pandas matplotlib seaborn openpyxl geopandas
- conda activate PI2
- conda create --name PI2-Seaborn python==3.11 ipykernel pandas matplotlib
- conda activate PI2-Seaborn
- conda install conda-forge::seaborn
- conda env export > environment.yml
- conda env create -f environment.yml

# Falta
- Actualizar población CABA
- Elegir 3er KPI

# Definición de kpi (Según copilot)
Un **KPI** (Key Performance Indicator o Indicador Clave de Rendimiento) es una métrica cuantitativa que indica el progreso hacia un objetivo. En el contexto del análisis de datos, los KPIs son fundamentales porque permiten a las empresas evaluar su rendimiento y tomar decisiones estratégicas basadas en datos.

Los KPIs no son simples métricas, sino que representan una 'brújula' estratégica para las organizaciones, permitiéndoles medir el éxito de sus iniciativas y estrategias con precisión y eficacia. Al ser cuidadosamente seleccionados y alineados con los objetivos empresariales, proporcionan una visión clara del rendimiento y el progreso¹.

Aunque a menudo se utilizan indistintamente, los KPIs y las métricas no son lo mismo. Las métricas son simplemente medidas estándar de cualquier proceso, como el número de visitas a una página web o la cantidad de ventas en un día. Por otro lado, un KPI es un indicador específico seleccionado por su relevancia crítica en el avance hacia un objetivo estratégico¹. Por ejemplo, un KPI podría ser el porcentaje de incremento en el tráfico de pago después de lanzar una nueva campaña de marketing.

En resumen, los KPIs están directamente alineados con los objetivos de la empresa y son indicativos del éxito o fracaso en áreas clave, mientras que las métricas pueden ser solo indicadores de rendimiento general sin una conexión directa con los objetivos estratégicos.
