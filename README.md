# Redes Neuronales para el Reconocimiento de Voz a partir de Espectrogramas
Este repositorio contiene el desarrollo completo del Proyecto I del curso de Inteligencia Artificial del Instituto Tecnológico de Costa Rica. El trabajo tiene un enfoque investigativo, experimental y formativo, orientado al aprendizaje y comprensión práctica de redes neuronales convolucionales aplicadas al problema de clasificación multiclase de sonidos ambientales a partir de sus representaciones log-Mel espectrogramas.

## Descripción del proyecto
El estudio busca evaluar y comprender la efectividad de distintas arquitecturas convolucionales en el reconocimiento automático de patrones acústicos. Se implementaron y compararon dos modelos desarrollados manualmente en PyTorch:

- **Modelo A**: Adaptación de `LeNet-5`, optimizada para imágenes RGB de 224×224 píxeles.
 
- **Modelo B**: Versión personalizada de `ResNet-18`, con conexiones residuales y regularización avanzada.

Ambos modelos fueron entrenados sobre el dataset público `ESC-50`, aplicando la técnica SpecAugment como método de aumento de datos en el dominio espectral.

## Metodología

El flujo experimental siguió un enfoque reproducible:

1. Conversión de los audios a espectrogramas log-Mel.

2. Aplicación de aumentación espectral (`SpecAugment`).

3. Entrenamiento y validación de los modelos bajo distintas configuraciones de hiperparámetros.

4. Registro y análisis de métricas con `Weights & Biases`.

