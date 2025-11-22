# Fase 3: Data Preparation

Este directorio está dedicado a la preparación de los datos para la fase de modelado, de acuerdo con el estándar CRISP-DM.

## Objetivo

Preparar y transformar los datos recopilados para su uso en modelado y análisis.

## Componentes de la carpeta

- `raw/`: Estructura reservada para datos brutos. No contiene datasets completos; el acceso y versionado de datos se gestiona mediante [DVC](https://dvc.org/).
- `processed/`: Contiene la estructura para resultados del preprocesamiento, generados a partir de los datos originales. Gestionados por DVC.
- `preprocessing/`: Scripts de limpieza, filtrado, reproyección, mosaico y segmentación de datos geoespaciales.
- `download/`: Scripts de interfaz para la adquisición automátizada desde APIs especializadas (por ejemplo, Google Earth Engine, SentinelHub).
- `dvc.yaml`: Pipeline de procesamiento definido en DVC que refleja y documenta cada paso en la preparación de datos.

## Gestión y versionado de datos

Toda la gestión de datasets, así como la sincronización entre colaboradores, se realiza utilizando DVC:

- **Agregar un nuevo dataset o resultado:**  

dvc add raw/NUEVO_DATASET/
dvc add processed/RESULTADO_PREPROCESO/
dvc push