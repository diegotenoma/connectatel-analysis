# 📊 Análisis de Clientes de ConnectaTel
Descripción del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica, utilizando información histórica disponible hasta el año 2024.

A través de técnicas de exploración, limpieza, análisis estadístico y segmentación de clientes, se busca identificar patrones de uso, detectar problemas de calidad de datos y generar recomendaciones que ayuden a la empresa a mejorar su oferta comercial y la toma de decisiones.

Objetivos
Explorar y comprender la estructura de los datos disponibles.
Detectar y corregir problemas de calidad de datos.
Analizar el comportamiento de uso de los clientes.
Identificar segmentos de usuarios según edad y nivel de consumo.
Detectar valores atípicos (outliers) relevantes para el negocio.
Generar insights y recomendaciones accionables para ConnectaTel.
Datasets Utilizados
1. plans.csv

Contiene información de los planes comerciales disponibles.

Variables principales:

Tipo de plan
Precio mensual
Minutos incluidos
Datos móviles incluidos
Costos por excedentes
2. users_latam.csv

Contiene información demográfica y contractual de los clientes.

Variables principales:

Identificador de usuario
Edad
Ciudad
Fecha de registro
Plan contratado
Fecha de cancelación (churn)
3. usage.csv

Contiene el detalle de uso de los servicios de telecomunicaciones.

Variables principales:

Identificador de usuario
Tipo de evento (llamada o mensaje)
Duración de llamadas
Longitud de mensajes
Fecha de uso
Etapas del Análisis
1. Carga y Exploración de Datos
Importación de librerías.
Carga de los datasets.
Revisión de estructura, dimensiones y tipos de datos.
2. Identificación de Problemas de Calidad
Detección de valores nulos.
Identificación de sentinels.
Revisión de valores inválidos.
Validación de fechas y registros fuera de rango.
3. Limpieza de Datos
Reemplazo de edades con valor sentinel (-999).
Corrección de fechas inválidas.
Tratamiento de valores faltantes.
Evaluación de datos MAR (Missing At Random).
4. Construcción del Perfil de Usuario
Agrupación de eventos por usuario.
Cálculo de:
Cantidad de mensajes.
Cantidad de llamadas.
Total de minutos consumidos.
Integración con la información demográfica.
5. Análisis Estadístico y Visualización
Estadísticas descriptivas.
Histogramas de distribución.
Comparación entre tipos de plan.
Identificación visual de patrones de comportamiento.
6. Detección y Tratamiento de Outliers
Uso de boxplots.
Cálculo de límites mediante método IQR.
Evaluación del impacto de los valores extremos.
7. Segmentación de Clientes
Segmentación por Uso
Bajo uso
Uso medio
Alto uso
Segmentación por Edad
Joven
Adulto
Adulto mayor
8. Elaboración de Insights Ejecutivos
Identificación de segmentos de mayor valor.
Evaluación de oportunidades comerciales.
Recomendaciones para optimización de planes.
Principales Hallazgos
Los usuarios entre 20 y 40 años se concentran principalmente en planes básicos.
Los usuarios de mayor edad muestran una mayor adopción de planes premium.
Se identificaron valores atípicos significativos en el consumo de minutos.
Existen oportunidades para diseñar estrategias de migración de clientes jóvenes hacia planes de mayor valor.
Requisitos

Para ejecutar el proyecto se recomienda:

Python 3.10+
pandas
numpy
matplotlib
seaborn
jupyter

Instalar dependencias:

pip install pandas numpy matplotlib seaborn jupyter
Cómo Ejecutar el Notebook
Opción 1: Google Colab
Abrir Google Colab.
Seleccionar File → Upload Notebook.
Cargar el archivo .ipynb.
Subir los datasets requeridos.
Actualizar las rutas de los archivos si es necesario.
Ejecutar las celdas en orden.
Opción 2: Jupyter Notebook
Clonar el repositorio:
git clone <URL_DEL_REPOSITORIO>
Entrar al directorio:
cd <NOMBRE_DEL_REPOSITORIO>
Ejecutar Jupyter:
jupyter notebook
Abrir el notebook del proyecto.
Ejecutar todas las celdas secuencialmente.
Guía de Reproducción
Obtener los archivos:
plans.csv
users_latam.csv
usage.csv
Colocarlos en la carpeta /datasets o actualizar las rutas en el notebook.
Ejecutar las secciones en el siguiente orden:
Exploración
Limpieza
Agregación de métricas
Estadísticas descriptivas
Visualizaciones
Segmentación
Insights ejecutivos
Verificar que los gráficos y tablas se generen correctamente.
Revisar las conclusiones finales para interpretar los resultados del análisis.
Autor

Diego Tenorio Martínez

Proyecto académico de análisis de datos utilizando Python, Pandas, NumPy, Matplotlib y Seaborn.
