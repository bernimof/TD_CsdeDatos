# M6 Proyecto Aprendizaje de Máquina Supervisado - Predicción inteligente de Gasto en Clientes E-commerce

---

## 🇨🇱 🇪🇸 Objetivo
Este proyecto diseña e implementa un modelo predictivo de **regresión supervisada** para estimar el **monto promedio de compra** de clientes de una empresa de e-commerce, a partir de variables demográficas y de comportamiento en el sitio web.

## Métodos
a) **Preprocesamiento** de datos: imputación de valores nulos, detección de outliers (IQR), codificación con variables dummy y escalamiento con StandardScaler.

b) **Modelos entrenados y comparados**:
  - Regresión Lineal
  - Regresión Polinomial
  - Regularización con Ridge y Lasso (alpha óptimo con GridSearchCV)
  - GradientBoostingRegressor (optimizado con GridSearchCV)

c) **Evaluación** con métricas de regresión: MAE, MSE, RMSE y R².

d) **Validación cruzada** K-Fold (K=5) para estimar robustez y estabilidad de los modelos.

e) **Ingeniería de características**: creación de 4 nuevas variables (engagement, ratio_conversion, recencia_inv, carrito_cupon) para capturar relaciones no lineales.

---

## 🇺🇸 🇬🇧 Objective
This project designs and implements a **supervised regression** predictive model to estimate the **average purchase amount** of e-commerce customers, based on demographic and website behavior variables.

## Methods
a) **Data preprocessing**: null value imputation, outlier detection (IQR), dummy encoding and StandardScaler normalization.

b) **Models trained and compared**:
  - Linear Regression
  - Polynomial Regression
  - Ridge and Lasso regularization (optimal alpha with GridSearchCV)
  - GradientBoostingRegressor (optimized with GridSearchCV)

c) **Evaluation** with regression metrics: MAE, MSE, RMSE and R².

d) **K-Fold Cross Validation** (K=5) to estimate robustness and stability of the models.

e) **Feature Engineering**: creation of 4 new variables (engagement, ratio_conversion, recencia_inv, carrito_cupon) to capture non-linear relationships.

---

## 👤 Autor / Author

**Bernardita Ortega**  
GitHub: https://github.com/bernimof  
LinkedIn: https://www.linkedin.com/in/bernarditaortega