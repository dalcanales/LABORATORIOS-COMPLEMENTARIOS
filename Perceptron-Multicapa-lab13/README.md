# Laboratorio 13 - Perceptrón Multicapa para Predicción de Campañas Bancarias

## Universidad César Vallejo

### Curso

Sistemas Inteligentes

### Integrante

- Dalia Canadakes

## Descripción

En este laboratorio se desarrolló un modelo de Perceptrón Multicapa (MLP) utilizando el conjunto de datos Bank Marketing de la UCI Machine Learning Repository. El objetivo fue predecir si un cliente aceptará o no un depósito bancario a plazo a partir de sus características personales y financieras.

## Herramientas utilizadas

- Python
- Pandas
- Scikit-Learn
- Matplotlib
- Joblib
- UCI Machine Learning Repository

## Arquitectura utilizada

- Capa oculta 1: 16 neuronas
- Capa oculta 2: 8 neuronas
- Función de activación: ReLU
- Optimizador: Adam
- Early Stopping habilitado

## Resultados obtenidos

Durante la evaluación del modelo se obtuvieron métricas de Accuracy, Precision, Recall y F1-score, además de la matriz de confusión y la curva de pérdida del entrenamiento. Posteriormente, se compararon tres arquitecturas distintas para determinar cuál ofrecía un mejor rendimiento.

## Comparación de arquitecturas

| Arquitectura | Accuracy | Precision | Recall | F1-score |
|--------------|----------|-----------|--------|----------|
| (8,) | 0.9028 | 0.6466 | 0.3724 | 0.4726 |
| (16,8) | 0.9005 | 0.6184 | 0.3900 | 0.4784 |
| (32,16,8) | **0.9053** | **0.6252** | **0.4751** | **0.5400** |

## Arquitectura seleccionada

La arquitectura **(32,16,8)** fue seleccionada por presentar el mejor desempeño general, obteniendo el mayor Accuracy, Recall y F1-score entre las tres configuraciones evaluadas.

## Archivos del proyecto

- lab13_mlp.ipynb
- mlp_bank_marketing_model.joblib

## Conclusión

El Perceptrón Multicapa demostró ser una alternativa adecuada para resolver problemas de clasificación en campañas bancarias. La comparación entre arquitecturas permitió comprobar que una red con mayor capacidad puede mejorar el desempeño del modelo siempre que no presente sobreajuste, logrando un equilibrio entre precisión y capacidad de generalización.