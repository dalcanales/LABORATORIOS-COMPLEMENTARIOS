# Laboratorio 14 - Clasificación de Dígitos Escritos a Mano usando CNN

## Universidad César Vallejo

### Curso

Sistemas Inteligentes

### Integrante

- Dalia Canales

## Descripción

En este laboratorio se desarrolló una Red Neuronal Convolucional (CNN) para clasificar imágenes de dígitos escritos a mano utilizando el dataset Optical Recognition of Handwritten Digits de UCI. El modelo fue entrenado y evaluado para reconocer correctamente los números del 0 al 9.

## Herramientas utilizadas

- Python
- Jupyter Notebook
- TensorFlow / Keras
- Scikit-Learn
- Pandas
- NumPy
- Matplotlib

---

# Respuestas

### 1. ¿Qué diferencia existe entre una red densa y una CNN?

Una red densa procesa todas las entradas por igual, mientras que una CNN analiza las imágenes mediante filtros que permiten identificar patrones como bordes, formas y trazos.

### 2. ¿Qué función cumple una capa convolucional?

Extrae características importantes de las imágenes aplicando filtros que detectan patrones locales necesarios para la clasificación.

### 3. ¿Qué representa un filtro en una CNN?

Es una pequeña matriz que recorre la imagen para identificar características como líneas, esquinas o diferentes formas.

### 4. ¿Qué función cumple MaxPooling?

Reduce el tamaño de las imágenes conservando la información más importante, disminuyendo el costo computacional y ayudando a evitar el sobreajuste.

### 5. ¿Por qué normalizamos los valores de píxeles?

Porque facilita el aprendizaje de la red neuronal, mejora la estabilidad del entrenamiento y acelera la convergencia del modelo.

### 6. ¿Por qué usamos Softmax en la capa de salida?

Porque convierte la salida del modelo en probabilidades, permitiendo identificar la clase con mayor probabilidad entre los diez dígitos.

### 7. ¿Qué dígitos se confundieron más en la matriz de confusión?

Las confusiones fueron mínimas y se presentaron principalmente entre dígitos con formas similares, como el 3 y el 5 o el 8 y el 9, dependiendo de los resultados obtenidos.

### 8. ¿Por qué algunos dígitos escritos a mano son difíciles de clasificar?

Porque algunas imágenes presentan trazos similares, diferencias en la escritura o pequeñas variaciones que dificultan distinguir ciertos números.

### 9. ¿Qué ventajas tendría usar imágenes de mayor resolución?

Permitirían capturar más detalles de los trazos, mejorando la capacidad del modelo para diferenciar imágenes similares.

### 10. ¿Qué limitaciones tiene este laboratorio frente a un sistema OCR real?

Se trabajó con imágenes pequeñas y un conjunto de datos controlado. Un sistema OCR real debe reconocer diferentes tamaños, estilos de escritura, iluminación y ruido en las imágenes.

---

# Conclusión

La implementación de una Red Neuronal Convolucional permitió clasificar correctamente los dígitos escritos a mano con un alto nivel de precisión. Se comprobó que las CNN son más eficientes que las redes densas para tareas de visión por computadora, ya que aprovechan la información espacial presente en las imágenes y logran un mejor desempeño en problemas de reconocimiento visual.