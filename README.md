# Detección de Alzheimer a partir de Imágenes Médicas con Redes Neuronales Convolucionales

Este proyecto implementa un modelo de red neuronal convolucional (CNN) utilizando la arquitectura ResNet50 y una arquitectura CNN personalizada para la detección del Alzheimer a partir de imágenes médicas. El objetivo es desarrollar una herramienta de ayuda para el diagnóstico, que clasifique las imágenes en diferentes etapas de la enfermedad o las identifique como normales.

## Tabla de Contenidos
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Propuesta de Solución](#propuesta-de-solución)
- [Requisitos](#requisitos)
- [Instalación](#instalación-de-dependencias)
- [Utilización del Proyecto](#utilización-del-proyecto)

## Descripción del Proyecto
El Alzheimer es una enfermedad neurodegenerativa que afecta a millones de personas en todo el mundo. La detección temprana es crucial para mejorar la calidad de vida de los pacientes y planificar un tratamiento adecuado. Este proyecto aplica técnicas de visión por computadora con modelos de aprendizaje profundo para clasificar imágenes cerebrales en distintas categorías (normal, leve, moderado y severo), basándose en el análisis de patrones en las imágenes de resonancia magnética (MRI).

## Propuesta de Solución
La propuesta mostrada por el grupo es de realizar modelos de redes neuronales convolucionales cuya entrada sean imágenes de resonancia magnética del cerebro humano y que sea capaz de clasificar la enfermedad de 
Alzheimer en cuatro categorías: No Demencia, Demencia Muy Leve, Demencia Leve y Demencia Moderada. Utilizando también técnicas de data augmentation y un balanceo de datos.

El proyecto incluye tres modelos:
1. **Modelo CNN Personalizado**: Una arquitectura CNN desarrollada desde cero, adaptada para trabajar con imágenes de una sola canal (escala de grises) y optimizada para detectar patrones en MRI.
2. **Modelo Basado en ResNet50**: Utiliza una arquitectura preentrenada de ResNet50 y está ajustado a nuestro conjunto de datos para la clasificación de imágenes médicas.
3. **Modelo Basado en MobileNetV2**: Utiliza una arquitectura preentrenada de ResNet50 y está ajustado a nuestro conjunto de datos para la clasificación de imágenes médicas.

## Requisitos
Para ejecutar este proyecto, necesitarás las siguientes bibliotecas y paquetes:
- **Python 3.x:**
  Lenguaje de programación en el que se desarrolló el proyecto.
  
- **PyTorch:**
  La librería principal para implementar la CNN, pues facilita la creación de modelos de Deep Learning, procesamiento de datos y aceleración por GPU.

- **Torchvision:**
  Se empleó para las transformaciones de imágenes mediante *transforms*.
  
- **TensorFlow:**
  Plataforma robusta para la creación de modelos de Deep Learning. Gestiona grandes volúmenes de datos, lo que permite un mejor procesamiento y también
  una buena aceleración por GPU.
  
- **Keras:**
  API de alto nivel integrada a Tensorflow, ayudó a simplificar los modelos por medio de una interfaz intuitiva y flexible, estructurando capas de la CNN de forma modular
  y ajustes de hiperparámetros.

- **SHAP (SHapley Additive exPLanations):**
  Utilizado para evaluar la interpretabilidad de los modelos, visualizando áreas específicas de las imágenes que influyeron en la decisión de clasificación del modelo.

- **Kaggle:**
  Se obtuvo el conjunto de datos gracias a kagglehub, permitiendo descargar datasets desde Kaggle, facilitando así la gestión de datos y el acceso a ellos.
  
- **Matplotlib:**
  Utilizado para la visualización de imágenes y de los resultados de interpretabilidad.

## Instalación de Dependencias
Instala las dependencias usando:
```bash
pip install -r requirements.txt
```

## Utilización del Proyecto

1. Coloca las imágenes en la carpeta data/ en subdirectorios organizados por clase.
2. Ejecutar notebook de proyecto, primero importando las librerías a utilizar.
3. Procesar y balancear la data utilizada mediante las celdas de procesamiento y balanceo de datos.
4. Generar y entrenar los modelos con su respectiva arquitectura.
5. Revisar las métricas, evaluar el rendimiento de las CNN e interpretar los gráficos generados.
