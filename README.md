# Movilidad urbana y economía | Análisis exploratorio (2024)

**Proyecto académico de Data Analytics (TripleTen)** · Python, pandas y Matplotlib

## Objetivo
Explorar la relación entre la congestión del tráfico urbano y los indicadores económicos de distintas ciudades. El análisis contrasta medidas de movilidad con PIB per cápita y otros indicadores para estudiar patrones; **no establece causalidad**.

## Datos
- `tomtom_traffic.csv`: indicadores de congestión y tiempos de desplazamiento.
- `oecd_city_economy.csv`: indicadores económicos por ciudad y año.

Los datos se cargan desde rutas `/datasets/` del entorno académico y **no están incluidos** en este repositorio. Para reproducir el análisis se necesitan los CSV originales o actualizar las rutas.

## Metodología
1. Importación y revisión de tipos de datos, valores faltantes y formatos.
2. Filtrado de observaciones del año 2024.
3. Agregación de indicadores de tráfico por ciudad, país y año con `groupby`.
4. Combinación de tráfico y economía por ciudad y año mediante un `merge` de las fuentes.
5. Visualizaciones exploratorias de distribuciones, congestión e indicadores económicos con pandas/Matplotlib.
6. Preparación de una exportación CSV limpia para análisis posterior.

## Hallazgos exploratorios
- En la muestra del ejercicio, el análisis identifica **Abu Dhabi** como ciudad con el mayor retraso promedio de tráfico.
- Al observar el PIB per cápita frente a congestión, no se encuentra una relación creciente uniforme: algunas ciudades con PIB alto registran congestión moderada o relativamente baja.
- Estos hallazgos son **descriptivos y limitados a los datos de la actividad**; no demuestran impacto del tráfico sobre la economía.

## Evidencia técnica
**[Abrir notebook original con código, visualizaciones y comentarios](S5%20ladb_mobility_economy_project_student-2.ipynb)**

[Ver notebook en GitHub](https://github.com/martinatn95-wq/analysis-everpeak/blob/main/S5%20ladb_mobility_economy_project_student-2.ipynb)

## Ejecución
1. Abre el notebook en Jupyter o Google Colab.
2. Instala las dependencias necesarias: `pandas`, `numpy`, `matplotlib` y `seaborn` si se utilizan en las celdas.
3. Proporciona los CSV de origen, ajusta sus rutas y ejecuta las celdas en orden.

**Limitaciones:** sin los CSV originales no se ha verificado una ejecución íntegra fuera del entorno del curso. El notebook incluye instrucciones y respuestas de práctica; algunas secciones de resumen ejecutivo permanecen como plantilla.

## Autor
Martín Alejandro Toledo Nieto · [Perfil GitHub](https://github.com/martinatn95-wq) · [LinkedIn](https://www.linkedin.com/in/martin-toledo-da-cpt/)
