# Detección de Alzheimer a partir de Imágenes Médicas con Redes Neuronales Convolucionales

Este proyecto implementa un modelo de red neuronal convolucional (CNN) utilizando la arquitectura ResNet50 y una arquitectura CNN personalizada para la detección del Alzheimer a partir de imágenes médicas. El objetivo es desarrollar una herramienta de ayuda para el diagnóstico, que clasifique las imágenes en diferentes etapas de la enfermedad o las identifique como normales.

## Tabla de Contenidos
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Requisitos](#requisitos)
- [Uso](#uso)
- [Resultados](#resultados)

## Descripción del Proyecto
El Alzheimer es una enfermedad neurodegenerativa que afecta a millones de personas en todo el mundo. La detección temprana es crucial para mejorar la calidad de vida de los pacientes y planificar un tratamiento adecuado. Este proyecto aplica técnicas de visión por computadora con modelos de aprendizaje profundo para clasificar imágenes cerebrales en distintas categorías (normal, leve, moderado y severo), basándose en el análisis de patrones en las imágenes de resonancia magnética (MRI).

El proyecto incluye tres modelos:
1. **Modelo CNN Personalizado**: Una arquitectura CNN desarrollada desde cero, adaptada para trabajar con imágenes de una sola canal (escala de grises) y optimizada para detectar patrones en MRI.
2. **Modelo Basado en ResNet50**: Utiliza una arquitectura preentrenada de ResNet50 y está ajustado a nuestro conjunto de datos para la clasificación de imágenes médicas.
3. **Modelo Basado en MobileNetV2**: Utiliza una arquitectura preentrenada de ResNet50 y está ajustado a nuestro conjunto de datos para la clasificación de imágenes médicas.


## Requisitos
Para ejecutar este proyecto, necesitarás las siguientes bibliotecas y paquetes:
- Python 3.x
- PyTorch
- TensorFlow
- Keras
- Matplotlib
- NumPy

Instala las dependencias usando:
```bash
pip install -r requirements.txt
```

## Uso

1. Coloca las imágenes en la carpeta data/ en subdirectorios organizados por clase.
2. Ejecutar notebook de proyecto
