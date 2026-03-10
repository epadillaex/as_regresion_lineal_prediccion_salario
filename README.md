# **Regresión Lineal Simple: Predicción de Salarios en Función de los Años de Experiencia**

## **Descripción**

Este proyecto tiene como objetivo construir un modelo de **regresión lineal simple** para predecir el salario de un empleado en función de sus años de experiencia. Utilizamos un conjunto de datos que contiene información sobre el salario y los años de experiencia de 30 empleados. El proyecto explora cómo aplicar la regresión lineal simple para modelar esta relación, realizar una evaluación del modelo y entender su rendimiento utilizando métricas comunes como el MSE, RMSE y \( R^2 \).

## **Contenido del Proyecto**

- **Introducción y Contexto**  
  Este proyecto se enfoca en la predicción del salario a partir de los años de experiencia laboral de un empleado. A pesar de ser un conjunto de datos pequeño, proporciona una excelente oportunidad para aprender cómo aplicar la regresión lineal simple y evaluar su desempeño.

- **Análisis Exploratorio de los Datos**  
  Se exploran y visualizan las variables para entender las relaciones entre los años de experiencia y el salario, identificando tendencias y posibles valores atípicos.  
  `Ejemplo de hallazgo`: Se observa una relación positiva entre los años de experiencia y el salario.

- **Preprocesamiento de los Datos**  
  Los datos se preparan para el modelo dividiéndolos en conjuntos de entrenamiento y validación. Dado que el conjunto de datos es pequeño, se realiza una división 80%-20% para la validación. 

- **Construcción del Modelo**  
  Se crea un modelo de regresión lineal simple utilizando **scikit-learn**. Este modelo se entrena para aprender la relación entre los años de experiencia y el salario, utilizando los datos de entrenamiento.

- **Entrenamiento y Validación del Modelo**  
  El modelo se entrena utilizando el conjunto de datos de entrenamiento y se valida utilizando el conjunto de validación para ajustar los parámetros del modelo y evitar el sobreajuste. Las métricas de rendimiento, como \( R^2 \), MSE se utilizan para evaluar el desempeño del modelo.


## **Requisitos**
   Python 3.11
   Librerías:
   - matplotlib==3.9.2
   - numpy==1.26.4
   - pandas==2.2.2
   - scikit-learn==1.5.1
   
   Puedes instalar las dependencias ejecutando:
   ```bash
       pip install -r requirements.txt
   ```
## **Estructura del Proyecto**
```
   ├── README.md                   # Descripción general del proyecto  
   ├── prediccion_salario.ipynb    # Código fuente del proyecto en Jupyter Notebook  
   ├── datasets/                   # Datos de entrada (contiene el conjunto de datos CSV de salarios)  
   └── requirements.txt            # Archivo con las dependencias necesarias para el proyecto
```
## **Resultados**

El modelo de regresión lineal simple logró un **\( R^2 \)** de aproximadamente 0.902, lo que indica que el modelo explica el 90.2% de la variabilidad en los salarios en función de los años de experiencia. Las métricas de error muestran un **RMSE** de 7,059.04 unidades monetarias, lo que sugiere que el modelo tiene un error relativamente bajo en las predicciones.

Para mejorar los resultados, se recomienda:
   - Probar un conjunto de datos más grande para mejorar la generalización.
   - Experimentar con una regresión lineal múltiple si se añaden más variables predictoras.
   - Ajustar los hiperparámetros del modelo y explorar diferentes enfoques de validación cruzada.


