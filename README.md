![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)


# <h1 align="center">**`Proyecto Individual 2`**

<p align="center">
<img src="https://www.ibm.com/blogs/client-voices/wp-content/uploads/2019/09/Glinnt.jpg"   
>
</p>


¡Bienvenidos a mi segundo proyecto individual!
  
En esta oportunidad pude poner en práctica mis habilidades en el campo de la predicción ya que el objetivo del trabajo era realizar un modelo de Machine Lerning que solucionara el problema planteado.



## 🏥**Descripción del problema**🏥

Cuando la hospitalización, o estancia hospitalaria, es prolongada constituye una preocupación a nivel mundial debido a que produce efectos negativos en el sistema de salud, aumentando los costos, generando deficiencia en la accesibilidad de prestación de servicios de salud, saturando las unidades de hospitalización y urgencias, por consiguiente, causa efectos adversos como lo son las enfermedades intrahospitalarias.
Es por eso que un importante Centro de Salud me ha contratado con el fin de poder predecir si un paciente tendrá una estancia hospitalaria prolongada o no, utilizando la información contenida en el dataset asociado, el cual recaba una muestra histórica de los pacientes, para poder administrar la demanda de camas en el hospital según la condición de los pacientes recientemente ingresados. En este caso, se considera estancia hospitalaria prolongada a la hospitalización de un paciente por más de 8 días.


## **Resolución del problema**

• Detectamos el problema;
  
•	Importamos los CSV train y test;
  
•	Realizamos un análisis exploratorio de los datos (EDA);
  
•	Comprobamos que no hayan datos nulos ni duplicados;
  
•	Se transforman los datos no numéricos para permitirle a los algoritmos realizar las predicciones;
  
• Utilizamos el método de correlación para saber, a partir de los datos dados, cuales son los Features más importantes para usar en nuestro modelo;
  
• Luego, declaramos las variables que utilizamos;
  
•	Realizamos el modelo con método de Clasificación ARBOL DE DESICION;
  
• Para saber que profundidad usar en el modelo se hace, a través de la librería de sklearn.model_selection, una cross_validate;
  
• Instanciamos el modelo con una profundidad (max_depth=4);
  
•	Lo entrenamos;
  
• Verifico la importancia de los feature elegidos con el método: feature_importances;
  
• Se realiza la matriz de confusión, luego se calcula la precisión (Accuracy) para las estadías hospitalarias largas:

                  $$ Accuracy=\frac{TP+TN}{P+N}$$ siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $P+N$ población total 
  
  y se realiza el recall:
  
                  $$ Recall=\frac{TP}{TP+FN}$$. Donde $TP$ son los verdaderos positivos y $FN$ los falsos negativos;
  
•	Hacemos el pipline de los datos necesarios ya que no debemos analizar los datos en los mismos sistemas donde se crean. Debido a que el proceso de analítica es  costoso computacionalmente, por lo que se separa para evitar perjudicar el rendimiento del servicio;
  
•	Por ultimo, se pone a disposición el Jupyter Notebook (.ipynb) en donde van a encontrar los comentarios con la fundamentación de la solución propuesta.

## **Conclusion*

La conclusión a la que he llegado es que: el *machine learning* es una herramienta  muy precisa que; en este caso, nos ayudó a predecir las estadías de hospitalización largas y cortas, aumentando la eficiencia del Centro de Salud ya que se puede planificar con antelación los registros y las admisiones hospitalarias de emergencia que se producen en el día a día.  
  








