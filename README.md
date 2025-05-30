# Proceso de Carga y Análisis de Datos - Avistamientos OVNI

## 1. Creación del Bucket y Carga del Archivo a Cloud Storage
Crear un bucket en Google Cloud Storage.
Cargar el archivo .csv correspondiente con los datos a analizar. (ufo_sighting)

## 2. Creación del Dataset en BigQuery
Crear un dataset en BigQuery llamado ovni.

## 3. Importación y Preparación de Datos
Importar el archivo .csv desde Cloud Storage hacia BigQuery.
Preparar los datos usando **DataPrep**:
  - Verificar valores nulos.
  - Identificar y corregir datos incorrectos.

## 4. Transformación de la Columna state/province
Cambiar el tipo de datos de la columna state/province a STRING.
Renombrar la columna a state_province (sin el caracter /).

## 5. Manejo de Valores Faltantes
Reemplazar valores faltantes por un valor personalizado.

## 6. Eliminación de Registros con Nulos Escasos
Eliminar filas con valores nulos en tablas donde estos sean escasos.

## 7. Cambio de Formato en la Columna date_time
Convertir el formato de la columna date_time a formato compatible con BigQuery.

## 8. Carga del Archivo Preparado
Cargar el archivo preparado con DataPrep en la tabla avistamientos del dataset ovni.

## 9. Consultas a la Tabla avistamientos
Realizar consultas SQL en BigQuery sobre la tabla avistamientos para obtener información relevante.

## 10. Generación de Gráficos en Looker Studio
Generar visualizaciones y gráficos solicitados utilizando **Looker Studio**.

## 11. Conclusion
La actividad permitió poner en práctica herramientas clave del ecosistema de Google Cloud como Cloud Storage, DataPrep, BigQuery y Looker Studio. A través de la limpieza de datos, análisis y visualización, se logró obtener una visión clara de los patrones de avistamientos de OVNIs en Estados Unidos.
