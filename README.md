# Modelos Ensemble en Machine Learning

Material del curso de **modelos ensemble** aplicado a ciencia de datos. Se estudian las técnicas de *Bagging*, *Boosting* y *Stacking*, junto con su aplicación en problemas de aprendizaje supervisado y no supervisado.

## Objetivos

Al finalizar el curso serás capaz de:

- Explicar por qué combinar varios modelos puede mejorar la precisión y la estabilidad de una predicción.
- Diferenciar los enfoques de *Bagging*, *Boosting* y *Stacking*.
- Entrenar, ajustar y evaluar modelos ensemble para clasificación y regresión.
- Comparar modelos mediante validación cruzada y métricas adecuadas al problema.
- Detectar sobreajuste, fuga de información y problemas de desbalance de clases.
- Interpretar la importancia de las variables y comunicar los resultados del modelo.

## Contenidos

### 1. Fundamentos

- Aprendizaje supervisado y no supervisado.
- Sesgo, varianza y error de generalización.
- Modelos base y combinación de predicciones.
- Partición de datos, validación cruzada y selección de métricas.

### 2. Bagging

- Bootstrap y agregación de modelos.
- Reducción de la varianza.
- Random Forest y Extra Trees.
- Importancia de variables y limitaciones de los árboles.

### 3. Boosting

- Entrenamiento secuencial de modelos débiles.
- AdaBoost y Gradient Boosting.
- XGBoost, LightGBM y CatBoost.
- Tasa de aprendizaje, número de estimadores y regularización.

### 4. Stacking y Voting

- Votación dura y blanda.
- Regresión y clasificación por apilamiento.
- Modelos de nivel superior y validación sin fuga de información.

### 5. Aplicación práctica

- Preparación y transformación de datos.
- Búsqueda de hiperparámetros.
- Evaluación, comparación y visualización de resultados.
- Interpretabilidad y puesta en producción.

## Requisitos

- Python 3.9 o superior.
- Conocimientos básicos de Python y análisis de datos.
- Nociones de probabilidad, estadística y aprendizaje automático.
- Jupyter Notebook o Visual Studio Code.

## Instalación

Se recomienda crear un entorno virtual para mantener aisladas las dependencias del curso:

```bash
python -m venv .venv
```

Activa el entorno virtual:

```bash
# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS/Linux
source .venv/bin/activate
```

Instala las dependencias del proyecto cuando esté disponible el archivo correspondiente:

```bash
python -m pip install --upgrade pip
python -m pip install numpy pandas scikit-learn matplotlib seaborn jupyter
```

Para trabajar con algoritmos de boosting adicionales:

```bash
python -m pip install xgboost lightgbm catboost
```

## Flujo de trabajo recomendado

1. Explorar y comprender el conjunto de datos.
2. Separar los datos de entrenamiento y prueba antes de ajustar transformaciones.
3. Construir un modelo base como referencia.
4. Entrenar distintos ensembles con validación cruzada.
5. Ajustar hiperparámetros usando únicamente los datos de entrenamiento.
6. Evaluar el modelo final sobre el conjunto de prueba.
7. Analizar errores, interpretabilidad y posibles mejoras.

## Buenas prácticas

- Usa `Pipeline` y `ColumnTransformer` para evitar fugas de información.
- Define la métrica antes de comparar modelos.
- Conserva un conjunto de prueba que no se utilice durante el ajuste.
- Compara siempre con un modelo base sencillo.
- Controla la complejidad del ensemble para evitar sobreajuste y tiempos innecesarios.
- Fija `random_state` cuando necesites resultados reproducibles.

## Resultado esperado

Al completar el curso deberás poder desarrollar un flujo completo de machine learning: desde la preparación de los datos hasta la selección, evaluación e interpretación de un modelo ensemble adecuado para un problema real.

