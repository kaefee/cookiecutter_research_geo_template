# Fase 2: Data Understanding

**Nota importante:**  
Este directorio NO almacena datasets completos.  
La gestión y trazabilidad de los datos geoespaciales utilizados en este proyecto se realiza mediante [DVC](https://dvc.org/), asegurando integridad, sincronización y reproducibilidad en colaboración.

## Componentes

- `sample_data/`: Ejemplos mínimos (imágenes, AOIs) para EDA rápida o documentación.
- `yyyymmdd_eda_notebook.ipynb`: Análisis exploratorio realizado únicamente sobre muestras ligeras.
- `scripts/`: Scripts para generación rápida de estadísticos y gráficos usando muestras.
- Todos los datasets utilizados para experimentación deben ser registrados y sincronizados con DVC.

## Acceso a datos reales

Para acceder a los datos de trabajo completos:
1. Configure el entorno según `common/environment.yml`.
2. Inicialice DVC y conecte el remoto apropiado:
