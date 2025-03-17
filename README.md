# AnalisisNoticiasSV

Este script en Python está diseñado para extraer, procesar y analizar noticias de un sitio web específico (`Diario Latino`). A continuación, se describen las características principales del código:

## Características Principales

1. **Extracción de Datos**:
   - Utiliza las librerías `requests` y `BeautifulSoup` para realizar web scraping y extraer información de noticias desde el sitio web `Diario Latino`.
   - Extrae URLs, títulos, autores, fechas de publicación, contenido y categorías de las noticias.

2. **Procesamiento de Datos**:
   - Limpia y transforma los datos extraídos, como la normalización de fechas y la eliminación de URLs duplicadas.
   - Almacena los datos en un DataFrame de `pandas` para facilitar su manipulación y análisis.

3. **Almacenamiento de Datos**:
   - Guarda los datos extraídos en múltiples formatos: CSV, JSON y un archivo de texto para facilitar su revisión y uso posterior.

4. **Análisis Exploratorio de Datos (EDA)**:
   - Realiza un análisis exploratorio de los datos, incluyendo estadísticas descriptivas y visualizaciones.
   - Genera gráficos de líneas y barras para mostrar la cantidad de noticias por fecha y categoría.

5. **Manejo de Errores**:
   - Incluye manejo de excepciones para gestionar errores durante la extracción de datos, como problemas de conexión o errores inesperados.

6. **Visualización de Datos**:
   - Utiliza `matplotlib` y `seaborn` para crear visualizaciones que ayudan a entender la distribución y tendencias de las noticias.

## Estructura del Código

- **Instalación de Librerías**: Importa las librerías necesarias como `requests`, `BeautifulSoup`, `pandas`, `json`, `os`, `datetime`, `matplotlib`, y `seaborn`.
- **Función de Fecha**: Define una función para convertir cadenas de texto en objetos `datetime`.
- **Extracción de URLs**: Recorre las páginas del sitio web y extrae las URLs de las noticias.
- **Procesamiento de Noticias**: Para cada URL de noticia, extrae y procesa el título, autor, fecha, contenido y categoría.
- **Creación de DataFrame**: Almacena los datos procesados en un DataFrame de `pandas`.
- **Almacenamiento**: Guarda los datos en archivos CSV, JSON y texto.
- **Análisis y Visualización**: Realiza análisis exploratorio y genera gráficos para visualizar los datos.

## Uso

Para utilizar este script, asegúrate de tener instaladas las librerías necesarias y ejecuta el código en un entorno Python. Los datos extraídos se guardarán en los archivos `Diario Latino.csv`, `Diario Latino.json`, y `Diario Latino.txt`.
