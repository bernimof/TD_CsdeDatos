# M7 Proyecto Aprendizaje de Máquina No Supervisado - Segmentador Inteligente de Clientes Minoristas

---

## 🇨🇱 🇪🇸 Objetivo
Este proyecto diseña e implementa un **pipeline completo de clusterización no supervisada** para segmentar clientes de una empresa de retail minorista, a partir de variables demográficas y de comportamiento de compra, sin etiquetas previas.

## Métodos
a) **Preprocesamiento** de datos: imputación de valores nulos (mediana para numéricas, moda para categóricas), detección de outliers (IQR), codificación con OrdinalEncoder y OneHotEncoder, y escalamiento con StandardScaler — resultado: 26 dimensiones.

b) **Reducción dimensional**:
  - PCA (2 componentes, 43.79% varianza explicada) — usado como entrada para clustering
  - t-SNE (perplexity=30) — usado exclusivamente para visualización de resultados

c) **Algoritmos de clusterización aplicados y comparados**:
  - K-Means (k=3 óptimo silueta, k=5 elegido por negocio)
  - DBSCAN (eps=1.4 y eps=1.45 elegido)
  - Agrupamiento Jerárquico Ward (k=3 y k=5 elegido, con dendrograma)

d) **Evaluación** con Coeficiente de Silueta y Método del Codo para selección de k óptimo.

e) **Perfilamiento de segmentos**: heatmap de variables numéricas y tabla de moda para variables categóricas por clúster.

---

## 🇺🇸 🇬🇧 Objective
This project designs and implements a **complete unsupervised clustering pipeline** to segment retail customers based on demographic and purchase behavior variables, without prior labels.

## Methods
a) **Data preprocessing**: null value imputation (median for numeric, mode for categorical), outlier detection (IQR), OrdinalEncoder and OneHotEncoder encoding, StandardScaler normalization — result: 26 dimensions.

b) **Dimensionality reduction**:
  - PCA (2 components, 43.79% explained variance) — used as input for clustering
  - t-SNE (perplexity=30) — used exclusively for results visualization

c) **Clustering algorithms applied and compared**:
  - K-Means (k=3 optimal silhouette, k=5 chosen for business)
  - DBSCAN (eps=1.4 and eps=1.45 chosen)
  - Hierarchical Ward Clustering (k=3 and k=5 chosen, with dendrogram)

d) **Evaluation** with Silhouette Coefficient and Elbow Method for optimal k selection.

e) **Segment profiling**: numeric heatmap and mode table for categorical variables per cluster.

---

## 📁 Dataset
**Customer Segmentation Classification** — Kaggle (kaushiksuresh147)  
🔗 https://www.kaggle.com/datasets/kaushiksuresh147/customer-segmentation

---

## 👤 Autora / Author
**Bernardita Ortega**  
GitHub: https://github.com/bernimof  
LinkedIn: https://www.linkedin.com/in/bernarditaortega
