# Proyecto de Fundamentos de Análisis y Cálculo Numérico

**Primera entrega — 2026-II**

## Integrantes

| Integrante | Código | Responsabilidad principal |
|---|---|---|
| **Laura Dayana Tascón** | 2438545-2724 | Notebook de fracturas óseas, interpretación de métricas, informe técnico y presentación |
| **Daniel Escobar Escobar** | 2437924-2724 | Notebooks con MNIST (partes 1, 2 y 3), instrucciones de ejecución y coordinación del repositorio |

## Descripción del proyecto

Este proyecto aborda los fundamentos de redes neuronales utilizando PyTorch, mediante ejercicios prácticos con tensores, construcción de redes neuronales y entrenamiento de modelos de aprendizaje profundo.

Se trabaja con dos conjuntos de datos: MNIST, para la clasificación de dígitos escritos a mano, y Bone Fracture Multi-Region X-ray Data, para la clasificación de radiografías en las categorías de fractura y sin fractura.

## Conjuntos de datos

### MNIST

- **Contenido:** imágenes de dígitos escritos a mano en escala de grises de 28×28 píxeles.
- **Clases:** 10 (dígitos del 0 al 9).
- **Uso en el proyecto:** partes 1, 2 y 3 de las guías (`Parte_1_Tensors`, `Parte_2_Neural_Networks` y `Parte_3_Training`).

### Bone Fracture Multi-Region X-ray Data

- **Contenido:** radiografías de distintas regiones del cuerpo, divididas en dos clases: `fractured` (con fractura) y `not fractured` (sin fractura).
- **Uso en el proyecto:** `Parte_2_3_Bone_Fracture.ipynb`.
- **Distribución de las imágenes:**

| Conjunto | fractured | not fractured | Total |
|---|---|---|---|
| Entrenamiento | 4606 | 4640 | 9246 |
| Validación | 337 | 492 | 829 |
| Prueba | 238 | 268 | 506 |

- **Observaciones:** el conjunto de validación tiene 829 imágenes, una más que las 828 indicadas por el autor, y está desbalanceado (337 vs. 492). Entrenamiento y prueba están casi balanceados.
- **Preprocesamiento aplicado:** escala de grises (1 canal), redimensionado a 64×64 píxeles y normalización a valores entre -1 y 1.
- **Estructura de carpetas:** cada conjunto (`train`, `val`, `test`) contiene una subcarpeta por clase. El notebook detecta automáticamente si el dataset está dentro de una o de dos carpetas `Bone_Fracture_Binary_Classification` anidadas.
- **Fuente:** [Fracture Multi-Region X-ray Data (Kaggle)](https://www.kaggle.com/datasets/bmadushanirodrigo/fracture-multi-region-x-ray-data/data).
- **Licencia:** Open Data Commons Attribution License (ODC-By) v1.0. Se debe dar atribución al autor.


## Contenido del repositorio

- `Parte_1_Tensors.ipynb`: operaciones y manipulación de tensores con PyTorch.
- `Parte_2_Neural_Networks.ipynb`: construcción y exploración de una red neuronal con MNIST.
- `Parte_3_Training.ipynb`: entrenamiento y evaluación de la red neuronal con MNIST.
- `Parte_2_3_Bone_Fracture.ipynb`: construcción, entrenamiento y evaluación de una red neuronal para clasificar radiografías de fracturas óseas.

## Tecnologías utilizadas

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Ejecución

1. Clonar el repositorio.
2. Crear y activar un entorno virtual de Python.
3. Instalar las dependencias necesarias.
4. Descargar los conjuntos de datos correspondientes y ubicarlos en las rutas configuradas en los notebooks.
5. Abrir los notebooks en Jupyter Notebook o Visual Studio Code y ejecutar las celdas en orden.

## Resultados

Los resultados de entrenamiento y evaluación, incluidas las métricas de desempeño y las visualizaciones generadas, se encuentran en los notebooks correspondientes.

## Repositorio

[Proyecto_FACN_Entrega1 en GitHub](https://github.com/zombiecommit/Proyecto_FACN_Entrega1)
