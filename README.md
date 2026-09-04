# Detección de Enfermedades en Hojas de Tomate

Este es el repositorio para la Evaluación Parcial N°1. El proyecto consiste en armar una red neuronal (Perceptrón Multicapa o MLP) para clasificar imágenes y detectar si una planta está enferma o no a partir del dataset PlantVillage.

## 1. Planteamiento del Problema y Objetivos
**El problema:** Las enfermedades en los cultivos de tomate hacen que se pierdan muchas cosechas y dinero. Detectarlas a tiempo a simple vista es difícil y requiere de expertos.
**El objetivo:** Entrenar un modelo MLP que pueda "mirar" una foto de una hoja de tomate y decirnos automáticamente si está sana o qué enfermedad específica tiene.

**Nuestras metas (KPIs):**
*   Lograr un **Accuracy (exactitud)** general por sobre el 80% en las pruebas.
*   Tener un buen **F1-Score** (mayor a 0.75) para asegurarnos de que el modelo no esté confundiendo hojas enfermas con hojas sanas.
*   Lograr que el modelo aprenda sin que colapse la memoria del entorno de trabajo (Google Colab).

## 2. Variante Elegida del Dataset
El dataset original de Kaggle (PlantVillage) trae más de 54.000 imágenes y 38 clases distintas de muchas plantas. 

Por eso, **acotamos el problema solo a las 10 clases correspondientes a las hojas de tomate**. Al achicar la cantidad de imágenes y enfocarnos en una sola planta, evitamos que el computador colapse y podemos evaluar de forma justa si el modelo MLP es capaz de aprender a detectar estas enfermedades.


## 3. Estructura de las Carpetas
El proyecto está ordenado de esta manera para mantener el orden:

```text
Plant_Village/
├── data/               # Aquí van las imágenes del dataset (no se suben a GitHub por el peso)
├── images/             # Aquí guardaremos gráficos de resultados (ej: matriz de confusión)
├── models/             # Aquí se guardará el modelo ya entrenado (.h5 o .keras)
├── notebooks/          # Aquí está el código ejecutable de Google Colab (.ipynb)
└── README.md           # Este archivo de presentación
