# Clasificacion de imágenes de radiografias de torax
Este repositorio contiene el desarrollo y entrenamiento de dos modelos de clasificación basados en redes neuronales profundas (ResNet50) para la detección automática de enfermedades pulmonares a partir de imágenes de radiografías torácicas. Los modelos están diseñados para detectar casos de COVID-19 y neumonía bacteriana en imágenes médicas, con el objetivo de proporcionar una herramienta complementaria en el diagnóstico clínico.

### Modelos desarrollados:

* Clasificador binario: Utiliza transfer learning con pesos preentrenados de DeepCOVID-XR, logrando un rendimiento destacado en la clasificación de pacientes con COVID-19 y neumonía bacteriana. El modelo alcanza una precisión del 98.30%, con una sensibilidad de 97.44%, lo que lo convierte en una herramienta prometedora para la detección temprana de estas enfermedades.

* Clasificador multiclase: Este modelo es capaz de diferenciar entre COVID-19, neumonía bacteriana y sujetos sanos. Aunque obtiene un accuracy global del 96%, presenta limitaciones en la detección de la clase neumonía bacteriana, con una baja sensibilidad de 0.44, lo que indica una alta tasa de falsos negativos para esta clase en particular.

### Características destacadas del proyecto:

* Uso de Transfer Learning: Se emplean modelos preentrenados (DeepCOVID-XR) para aprovechar representaciones de características aprendidas previamente y mejorar la precisión del modelo con un esfuerzo de entrenamiento reducido.
  
* Optimización de Hiperparámetros: Se realiza un ajuste minucioso de los parámetros del modelo para maximizar su rendimiento, priorizando la sensibilidad y la detección precisa de los casos positivos.
  
* Evaluación de Métricas: Se analizan diversas métricas, incluyendo accuracy, sensibilidad, especificidad y F1-score, para evaluar el rendimiento de los clasificadores tanto en el escenario binario como multiclase.
  
* Interpretabilidad: A través del análisis de mapas de activación, se explora cómo el modelo toma decisiones, enfocándose en las regiones pulmonares, lo cual es relevante desde el punto de vista clínico.
  
* Limitaciones y Futuro: Aunque el modelo binario ha demostrado ser efectivo en la clasificación de COVID-19 y neumonía bacteriana, es crucial realizar una validación adicional en entornos hospitalarios con datos externos y consultar con especialistas en radiología para garantizar la fiabilidad y la interpretación clínica adecuada. Para el clasificador multiclase, se requieren mejoras, especialmente en la detección de neumonía bacteriana, lo cual puede abordarse mediante técnicas de aumento de datos y la recopilación de más imágenes para esta clase.

* Uso en la práctica médica: El proyecto busca proporcionar una herramienta diagnóstica de apoyo que, junto con la evaluación de profesionales de la salud, pueda ayudar a la detección temprana de enfermedades pulmonares, contribuyendo así a mejorar los tiempos de diagnóstico y tratamiento.

Para más detalles sobre la implementación, consulta los el notebook .ipynb
