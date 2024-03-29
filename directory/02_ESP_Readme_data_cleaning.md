# Descripción General
Este script procesa datos brutos de estadísticas de jugadores de fútbol de varias temporadas. Involucra la lectura, limpieza, fusión y transformación de datos para su posterior análisis y aplicación.

# Prerrequisitos
- Python 3
- Biblioteca Pandas
- Biblioteca openpyxl (para manejar archivos de Excel)

# Archivos de Datos
- `player_stats_2018_2022_raw.xlsx`: Contiene estadísticas de jugadores para los años 2018-2022.
- `player_stats_2013_raw.xlsx`: Contiene estadísticas de jugadores para el año 2013.

# Pasos Clave en el Script
1. **Carga de Datos**: El script comienza cargando los datos de estadísticas de jugadores de las temporadas 2018-2022 y 2013 utilizando Pandas. Las rutas a estos archivos deben ajustarse según la estructura de archivos de tu sistema.

2. **Fusión de Datos**: Los datos de diferentes temporadas (2018-2022 y 2013) se combinan en un solo DataFrame.

3. **Limpieza de Datos**: El script limpia los datos reemplazando los valores NA con ceros.

4. **Selección de Columnas**: Se seleccionan columnas específicas para mantener en el conjunto de datos final.

5. **Renombrar Columnas**: Las columnas se renombran al español para una mejor comprensión en el contexto dado.

6. **Conversión de Tipos**: Se convierten ciertas columnas a tipos numéricos para un manejo adecuado de los datos.

7. **Mapeo de Posiciones**: Las posiciones detalladas de los jugadores se mapean a categorías de posición generales.

8. **Creación de ID Único**: Se crea un ID único para cada jugador basado en múltiples atributos.

9. **Procesamiento de Fechas**: Las fechas de nacimiento se convierten a datetime y se calcula la edad de los jugadores.

10. **Traducción de Datos**: Los nombres de competiciones y la lateralidad de los jugadores se traducen del inglés al español.

11. **Eliminación de Duplicados**: Se eliminan las filas duplicadas basadas en el ID único.

12. **Exportación de Datos**: Los datos procesados se exportan a un archivo Excel para su uso posterior.

# Nota sobre las Rutas de Archivos
Asegúrate de que las rutas a los archivos de Excel estén correctamente establecidas para coincidir con la estructura de directorios de tu sistema.

# Personalización
Siéntete libre de modificar el script para adaptarlo a tus necesidades específicas de procesamiento de datos.
