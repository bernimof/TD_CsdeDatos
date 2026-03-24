# M8 Fundamentos de Deep Learning - Clasificador Inteligente de Imágenes de Ropa (StyleNet)

---

## 🇨🇱 🇪🇸 Objetivo
Este proyecto diseña e implementa un **clasificador de imágenes de prendas de vestir** basado en redes neuronales profundas, para automatizar el etiquetado de productos en la plataforma de comercio electrónico StyleNet, reemplazando el proceso manual de categorización.

## Métodos

a) **Preprocesamiento** de datos: escalamiento de píxeles [0,255] → [0.0, 1.0] dividiendo por 255, reshape para MLP (60.000, 784) y CNN (60.000, 28, 28, 1), y codificación de etiquetas con `to_categorical` (one-hot encoding, 10 clases).

b) **Lección 1 – Red Neuronal Artificial**: definición teórica de arquitectura densa, identificación de capas, pesos, sesgos, funciones de activación (ReLU, Softmax, Sigmoid) y ciclo de entrenamiento (Forward Pass → Loss → Backpropagation).

c) **Lección 2 – Deep Learning**: investigación y documentación de arquitecturas (DNN, CNN, RNN, Autoencoders, Transformers), justificación de CNN sobre MLP para clasificación de imágenes, y selección de **Keras** como framework.

d) **Lección 3 – Red Neuronal Densa (MLP)**:
  - MLP Simple: `Input(784) → Dense(128, ReLU) → Dense(10, Softmax)` — optimizer Adam (lr=0.001), epochs=15, batch_size=64
  - MLP lr bajo: misma arquitectura con `Adam(lr=0.0001)` y batch_size=128 — comparativa de hiperparámetros.
  - Regularización: Dropout aplicado en versión elaborada.

e) **Lección 4 – Red Neuronal Convolutiva (CNN)**:
  - `Conv2D(32) → MaxPool → Conv2D(64) → MaxPool → Flatten → Dropout(0.5) → Dense(10, Softmax)`
  - Optimizer: Adam (lr=0.001), epochs=15, batch_size=64
  - Evaluación comparativa CNN vs MLP con `accuracy_score`

f) **Evaluación**: accuracy en test, matriz de confusión (`ConfusionMatrixDisplay`), reporte de clasificación por clase (`classification_report`) con precision, recall y F1-score.

g) **Predicciones visuales**: grid de 9 imágenes del test set con etiqueta real vs predicha (verde=correcto, rojo=error).

---

## 🇺🇸 🇬🇧 Objective
This project designs and implements a **clothing image classifier** based on deep neural networks, to automate product labeling on the StyleNet e-commerce platform, replacing the manual categorization process.

## Methods

a) **Data preprocessing**: pixel scaling [0,255] → [0.0, 1.0] by dividing by 255, reshape for MLP (60,000, 784) and CNN (60,000, 28, 28, 1), and label encoding with `to_categorical` (one-hot, 10 classes).

b) **Lesson 1 – Artificial Neural Network**: theoretical definition of dense architecture, identification of layers, weights, biases, activation functions (ReLU, Softmax, Sigmoid) and training cycle (Forward Pass → Loss → Backpropagation).

c) **Lesson 2 – Deep Learning**: research and documentation of architectures (DNN, CNN, RNN, Autoencoders, Transformers), justification of CNN over MLP for image classification, and selection of **Keras** as framework.

d) **Lesson 3 – Dense Neural Network (MLP)**:
  - Simple MLP: `Input(784) → Dense(128, ReLU) → Dense(10, Softmax)` — Adam optimizer (lr=0.001), epochs=15, batch_size=64
  - Low LR MLP: same architecture with `Adam(lr=0.0001)` and batch_size=128 — hyperparameter comparison
  - Regularization: Dropout applied in elaborated version

e) **Lesson 4 – Convolutional Neural Network (CNN)**:
  - `Conv2D(32) → MaxPool → Conv2D(64) → MaxPool → Flatten → Dropout(0.5) → Dense(10, Softmax)`
  - Optimizer: Adam (lr=0.001), epochs=15, batch_size=64
  - Comparative evaluation CNN vs MLP using `accuracy_score`

f) **Evaluation**: test accuracy, confusion matrix (`ConfusionMatrixDisplay`), classification report per class (`classification_report`) with precision, recall and F1-score.

g) **Visual predictions**: grid of 9 test set images with real vs predicted label (green=correct, red=error).


---

## 📁 Dataset
**Fashion-MNIST** — Keras Datasets  
🔗 https://keras.io/api/datasets/fashion_mnist/

10 categories: T-shirt/Top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot  
70.000 grayscale images (28×28 px) — 60.000 train / 10.000 test


---

## 👤 Autora / Author
**Bernardita Ortega**  
GitHub: https://github.com/bernimof  
LinkedIn: https://www.linkedin.com/in/bernarditaortega
