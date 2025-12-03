# Redes Neuronales – Modulo 5
## Integrantes
- Juan David Meza
- Andres Mauricio Avilan

# **Ejercicio 1 — Redes neuronales desde cero (NAND y XOR)**

En este ejercicio se implementaron dos redes neuronales **sin usar TensorFlow**, siguiendo la estructura del programa `Clase_NNA3`.  
Todo el entrenamiento se realiza mediante:

- Propagación hacia adelante (Forward propagation)
- Retropropagación del error (Backpropagation)
- Función de activación sigmoide
- Descenso del gradiente
- Dos capas ocultas

### Archivos:
- **`nand_network.ipynb`**  
  Red neuronal con dos capas ocultas entrenada para aprender la compuerta **NAND**.
  <img width="208" height="142" alt="image" src="https://github.com/user-attachments/assets/1e69ba29-9956-4db8-b3df-264fca52ed0b" /> 
  
- **`xor_network.ipnb`**  
Misma arquitectura, entrenada para aprender la función **XOR*:  
<img width="208" height="136" alt="image" src="https://github.com/user-attachments/assets/fc869622-7124-4f74-aebc-26bedb35c993" />

# **Ejercicio 2 — Clasificación Fashion-MNIST con TensorFlow**

Este ejercicio implementa una red neuronal multicapa usando **TensorFlow/Keras** para clasificar prendas del dataset **Fashion-MNIST**.

### Archivo:
- **`fashion_mnist_classifier.py`**

<img width="601" height="589" alt="image" src="https://github.com/user-attachments/assets/e6f6efe6-fc36-4fb6-8f01-1a9cd47fb7df" />


Se logra una precisión aproximada entre **87% y 90%**, dependiendo de la cantidad de épocas.

- La normalización mejora la estabilidad del entrenamiento.  
- El uso de funciones ReLU en capas ocultas acelera el aprendizaje.  
- Softmax + crossentropy son fundamentales para clasificación multiclase.  
- TensorFlow automatiza el cálculo de gradientes y facilita el desarrollo.

---

# **Ejercicio 3 — Red neuronal sobre dataset real (Iris Dataset)**

Para este ejercicio se escogió el dataset **Iris**, disponible en Kaggle/Sklearn. Se construye una red neuronal para clasificar tres tipos de flores.

### Archivo:
- **`iris_classifier.py`**

<img width="764" height="87" alt="image" src="https://github.com/user-attachments/assets/4649a646-be42-432d-80e2-fd8b1ad93a27" />

### Resultados:
El modelo logra una precisión entre **95% y 98%** en el conjunto de prueba.

- La selección adecuada de características facilita el entrenamiento.  
- Redes pequeñas son suficientes para datasets simples.  
- El preprocesamiento (normalización) es clave para estabilidad del gradiente.  
