![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)


# <h1 align="center">**`Proyecto Individual 2`**

<p align="center">
<img src="https://www.ibm.com/blogs/client-voices/wp-content/uploads/2019/09/Glinnt.jpg"   
>
</p>


¡Bienvenidos a mi segundo proyecto individual! 
En esta oportunidad puse en práctica mis habilidades en el campo de la predicción. El objetivo de este trabajo era realizar un modelo de Machine Lerning para solucionar el problema planteado.



## 🏥 **Estancia hospitalaria** 🏥

La hospitalización, o estancia hospitalaria, cuando es prolongada constituye una preocupación a nivel mundial debido a sus efectos negativos en el sistema de salud, aumentando los costos, generando deficiencia en la accesibilidad de prestación de servicios de salud, saturación de unidades de hospitalización y urgencias, por consiguiente, mayores efectos adversos como lo son las enfermedades intrahospitalarias.

El estudio de los procesos de atención en salud, así como el conocimiento de las características y perfiles de los usuarios con el objetivo de predecir la ocupación hospitalaria, es uno de los aspectos al que las autoridades de salud han prestado gran interés, pues permite no sólo garantizar los recursos necesarios para la atención del paciente, sino realizar ajustes respecto a la oferta y demanda de los servicios de salud y los implementos asociados.

## **Descripción del problema**

Un importante Centro de Salud me ha contratado con el fin de poder predecir si un paciente tendrá una estancia hospitalaria prolongada o no, utilizando la información contenida en el dataset asociado, la cual recaba una muestra histórica de sus pacientes, para poder administrar la demanda de camas en el hospital según la condición de los pacientes recientemente ingresados. 
Para esto, se define que un paciente posee estancia hospitalaria prolongada si ha estado hospitalizado más de 8 días. Por lo que debe generar dicha variable categórica y luego categorizar los pacientes según las variables que usted considere necesarias, justificando dicha elección. 


## **Resolución del problema**

• Detectamos el problema.
•	Importamos los CSV train y test.
•	Realizamos un análisis exploratorio de los datos (EDA).
•	Comprobamos que no hayan datos nulos ni duplicados.
•	Se transforman los datos no numéricos para permitirle a los algoritmos realizar las predicciones.
• Utilizamos el método de correlación para saber, a partir de los datos dados, cuales son los Features más importantes para usar en nuestro modelo.
• Luego, declaramos las variables que utilizamos.
•	Entrenamos y predecimos utilizando el modelo con método de Clasificación ARBOL DE DESICION.
• Para saber que profundidad usar en el modelo se hace, a través de la librería de sklearn.model_selection, una cross_validate
• Instanciamos el modelo con una profundidad (max_depth=4)
•	Lo entrenamos.
• Verifico la importancia de los feature elegidos con el método: feature_importances
• Se realiza la matriz de confusión, se saca la exactitud del modelo, la precisión (Accuracy) para las estadías hospitalarias largas.

$$ Accuracy=\frac{TP+TN}{P+N}$$

siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $P+N$ población total y el recall $$ Recall=\frac{TP}{TP+FN}$$


Donde $TP$ son los verdaderos positivos y $FN$ los falsos negativos.
•	Hacemos el pipline de los datos necesarios ya que no debemos analizar los datos en los mismos sistemas donde se crean. Debido a que el proceso de analítica es  costoso computacionalmente, por lo que se separa para evitar perjudicar el rendimiento del servicio. 
•	Por ultimo, recuerden que en el Jupyter Notebook (.ipynb) van a encontrar los comentarios con la fundamentación de la solución propuesta.

## **Criterio de evaluación**



## **Métrica a utilizar**

​







