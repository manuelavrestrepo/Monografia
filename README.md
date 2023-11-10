# Monografia
## Titulo: Complementariedad de los recursos de generación de energía solar, eólica e hídrica en Colombia
## Autor: Manuela Velásquez Restrepo

## Descripción del Proyecto

El proyecto se enfoca en evaluar la complementariedad de los recursos de generación de energía solar, eólica e hídrica en el contexto del sector eléctrico colombiano, donde la generación hidráulica representa una parte significativa de la generación total del país. Se emplea la técnica de Funciones Ortogonales Empíricas (EOF) y análisis de correlación en diferentes escalas temporales para caracterizar climáticamente las variables e identificar la complementariedad entre los recursos.

### Estructura del Repositorio

- **/DatosCrudos**: Contiene una pequeña muestra de los datos crudos necesarios para la evaluación, dado que los datos completos pesan aproximadamente 75Gb.
- **/DatosTransformados**: Contiene los archivos NetCDF de los datos transformados, matrices mensuales, ciclos anuales, ciclos diurnos y matrices promedio de largo plazo.
- **/scripts**: Incluye el código fuente (`Monografia_ME03`) para la lectura y transformación de datos.


## Código - Monografia_ME03

El código `Monografia_ME03` aborda la primera fase del proyecto, que se enfoca en la lectura y transformación de los datos crudos necesarios para la evaluación. Para llevar a cabo este proceso, se emplea información climática de radiación solar, velocidad del viento y precipitación. Además, se utiliza el Índice Oceánico de El Niño (ONI) para identificar las fases del Fenómeno El Niño Oscilación del Sur (ENSO).

### Contenido

### 1. Importar Librerías <a name="importar-librerías"></a>

Se importan las librerías necesarias para el procesamiento y análisis de datos geoespaciales y climáticos.

### 2. Datos de Precipitación de CHIRPS <a name="datos-de-precipitación-de-chirps"></a>

Se cargan y procesan los datos de precipitación de CHIRPS, centrándose en la región de estudio en Colombia.

#### Precipitación Mensual Acumulada <a name="precipitación-mensual-acumulada"></a>

Se realiza un análisis de la precipitación mensual acumulada, mostrando la serie de tiempo.

#### Ciclo Anual Promedio de Precipitación <a name="ciclo-anual-promedio-de-precipitación"></a>

Se calcula y visualiza el ciclo anual promedio de precipitación en la región de estudio.

#### Precipitación Anual Acumulada <a name="precipitación-anual-acumulada"></a>

Se presenta la precipitación anual acumulada en forma de mapas.
### 3. Datos de Irradiación Global Horizontal (GHI) <a name="datos-de-irradiación-global-horizontal-ghi"></a>

Se obtienen y procesan los datos de GHI a partir de archivos NetCDF de la base de datos ERA5.

#### GHI Mensual Promedio <a name="ghi-mensual-promedio"></a>

Se realiza un análisis de la irradiación global horizontal, mostrando la serie de tiempo para un punto en particular.

#### Ciclo Anual Promedio de GHI <a name="ciclo-anual-promedio-de-ghi"></a>

Se calcula y visualiza el ciclo anual promedio de GHI en la región de estudio.

#### Ciclo Diurno de GHI <a name="ciclo-diurno-de-ghi"></a>

Se presenta el ciclo diurno promedio de GHI en una ubicación específica (por ejemplo, Medellín).

#### GHI Promedio Diario <a name="ghi-promedio-diario"></a>

Se muestra la irradiación global horizontal promedio diaria acumulada en forma de mapas.

### 4. Datos del Índice Oceánico de El Niño (ONI) <a name="datos-de-irradiación-global-horizontal-ghi"></a>

Se obtiene el ONI a partir de archivo .xlsx construido a partir de la base de datos de la NOAA
