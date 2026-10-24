# Marketing bancario: clasificación de suscripción a depósitos

Proyecto grupal desarrollado para el curso de Machine Learning del Magíster en Data Science de la Universidad del Desarrollo. El objetivo académico es explorar y comparar métodos de clasificación para estimar si una persona contratará un depósito a plazo después de una campaña telefónica.

**Integrantes:** Adrian Espinoza, Dante Aguirre y Sofia Alanis.

## Alcance

El trabajo recorre análisis exploratorio, preparación de datos y comparación de modelos supervisados, junto con técnicas de reducción de dimensionalidad y clustering descritas en el enunciado del proyecto. Los resultados son exploratorios y corresponden a una entrega académica; no representan una evaluación en producción ni validan impactos comerciales.

El conjunto de datos Bank Marketing de UCI contiene 45.211 registros. El proyecto incluye una versión procesada en `data/clean/bank_marketing_clean.csv`.

## Estructura

- `notebooks/01_eda_analysis.ipynb`: análisis exploratorio.
- `notebooks/02_preprocessing.ipynb`: preparación de datos.
- `notebooks/03_ml_model.ipynb`: entrenamiento y evaluación de modelos.
- `data/clean/bank_marketing_clean.csv`: datos procesados.
- `figures/`: gráficos generados para los análisis.
- `assets/`: enunciado del proyecto.

## Cómo revisar

Puedes abrir los notebooks directamente desde GitHub. Para obtener una copia local:

```bash
git clone https://github.com/danteaguirreb/tarea_final_ml_marketing_bancario.git
cd tarea_final_ml_marketing_bancario
```

El repositorio incluye `requirements.txt`, pero ese archivo conserva rutas de instalación específicas del entorno donde se generó y puede no funcionar en otros equipos. Por eso no se presenta como una instalación reproducible: revisa las importaciones de los notebooks y ajusta las dependencias a tu entorno antes de ejecutarlos.

## Nota metodológica

La variable `duration` registra la duración de la llamada y solo se conoce una vez que esta termina. Por tanto, no debe usarse para una predicción previa al contacto. Cualquier evaluación que la incluya debe interpretarse considerando esa limitación.

## Fuente de datos

Moro, S., Cortez, P. y Rita, P. (2014). *A Data-Driven Approach to Predict the Success of Bank Telemarketing*. UCI Machine Learning Repository: [Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing).

## Material complementario

- [Enunciado del proyecto](./assets/enunciado_proyecto_completo.md)
- [Repositorio de ejercicios del curso](https://github.com/danteaguirreb/machine_learning)
