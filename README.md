# 📁 Parte II: Preprocesamiento y Optimización

## 🎯 Objetivo
Realizar el preprocesamiento y la optimización de modelos de machine learning para el dataset seleccionado. El objetivo es elegir la técnica más adecuada y ajustar sus hiperparámetros para obtener el mejor rendimiento posible.

---

## 🧼 Preprocesamiento de Datos

- **Limpieza de datos:**
  - Imputación o eliminación de valores nulos según relevancia y tipo de variable.
  - Identificación y tratamiento de outliers con transformaciones o filtrado.

- **Transformación de columnas:**
  - Aplicación de `ColumnTransformer` para escalar y codificar de forma diferenciada.
  - Codificación categórica con `OneHotEncoder`.
  - Escalado numérico con `StandardScaler`.

- **Pipeline completo:**
  - Uso de `sklearn.Pipeline` para encapsular todo el preprocesamiento y garantizar reproducibilidad.

---

## 🤖 Selección de Técnica de Machine Learning

- Entrenamiento inicial con modelos base:
  - `LinearRegression`
  - `KNeighborsRegressor`
  - `RandomForestRegressor`


- Evaluación con validación cruzada (`cross_val_score`) usando `RMSE` y `R²`.
- Comparación objetiva para seleccionar el modelo con mejor rendimiento inicial.

---

## 🧠 Optimización de Hiperparámetros

- **GridSearchCV:**
  - Búsqueda exhaustiva del mejor conjunto de hiperparámetros.

- **RandomizedSearchCV:**
  - Búsqueda aleatoria para espacios amplios de hiperparámetros.

- **Optuna:**
  - Optimización avanzada 

---

## 📊 Evaluación de Modelos Optimizados

- Entrenamiento final con los mejores hiperparámetros.
- Evaluación sobre el conjunto de prueba (`RMSE`, `R²`).
- Comparativa directa con el modelo inicial.

```text
🔍 Comparativa:
Modelo Inicial     - RMSE: 9.92 | R²: 0.56
Modelo Optimizado  - RMSE: 4.06 | R²: 0.93
