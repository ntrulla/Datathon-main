![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)


# <h1 align="center">**`Proyecto Individual 2`**

<p align="center">
<img src="https://www.ibm.com/blogs/client-voices/wp-content/uploads/2019/09/Glinnt.jpg"   
>
</p>


隆Bienvenidos a mi segundo proyecto individual!
  
En esta oportunidad pude poner en pr谩ctica mis habilidades en el campo de la predicci贸n ya que el objetivo del trabajo era realizar un modelo de Machine Lerning que solucionara el problema planteado.



## 馃彞**Descripci贸n del problema**馃彞

Cuando la hospitalizaci贸n, o estancia hospitalaria, es prolongada constituye una preocupaci贸n a nivel mundial debido a que produce efectos negativos en el sistema de salud, aumentando los costos, generando deficiencia en la accesibilidad de prestaci贸n de servicios de salud, saturando las unidades de hospitalizaci贸n y urgencias, por consiguiente, causa efectos adversos como lo son las enfermedades intrahospitalarias.
Es por eso que un importante Centro de Salud me ha contratado con el fin de poder predecir si un paciente tendr谩 una estancia hospitalaria prolongada o no, utilizando la informaci贸n contenida en el dataset asociado, el cual recaba una muestra hist贸rica de los pacientes, para poder administrar la demanda de camas en el hospital seg煤n la condici贸n de los pacientes recientemente ingresados. En este caso, se considera estancia hospitalaria prolongada a la hospitalizaci贸n de un paciente por m谩s de 8 d铆as.


## **Resoluci贸n del problema**

鈥? Detectamos el problema;
  
鈥?	Importamos los CSV train y test;
  
鈥?	Realizamos un an谩lisis exploratorio de los datos (EDA);
  
鈥?	Comprobamos que no hayan datos nulos ni duplicados;
  
鈥?	Se transforman los datos no num茅ricos para permitirle a los algoritmos realizar las predicciones;
  
鈥? Utilizamos el m茅todo de correlaci贸n para saber, a partir de los datos dados, cuales son los Features m谩s importantes para usar en nuestro modelo;
  
鈥? Luego, declaramos las variables que utilizamos;
  
鈥?	Realizamos el modelo con m茅todo de Clasificaci贸n ARBOL DE DESICION;
  
鈥? Para saber que profundidad usar en el modelo se hace, a trav茅s de la librer铆a de sklearn.model_selection, una cross_validate;
  
鈥? Instanciamos el modelo con una profundidad (max_depth=4);
  
鈥?	Lo entrenamos;
  
鈥? Verifico la importancia de los feature elegidos con el m茅todo: feature_importances;
  
鈥? Se realiza la matriz de confusi贸n, luego se calcula la precisi贸n (Accuracy) para las estad铆as hospitalarias largas:

                  $$ Accuracy=\frac{TP+TN}{P+N}$$ siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $P+N$ poblaci贸n total 
  
  y se realiza el recall:
  
                  $$ Recall=\frac{TP}{TP+FN}$$. Donde $TP$ son los verdaderos positivos y $FN$ los falsos negativos;
  
鈥?	Hacemos el pipline de los datos necesarios ya que no debemos analizar los datos en los mismos sistemas donde se crean. Debido a que el proceso de anal铆tica es  costoso computacionalmente, por lo que se separa para evitar perjudicar el rendimiento del servicio;
  
鈥?	Por ultimo, se pone a disposici贸n el Jupyter Notebook (.ipynb) en donde van a encontrar los comentarios con la fundamentaci贸n de la soluci贸n propuesta.

## **Conclusi贸n*

La conclusi贸n a la que he llegado es que: el *machine learning* es una herramienta  muy precisa que; en este caso, nos ayud贸 a predecir las estad铆as de hospitalizaci贸n largas. Asi, se pudo aumentar la eficiencia del Centro de Salud ya que este puede saber con antelaci贸n cuales van a ser los registros y las admisiones hospitalarias de emergencia que se producen en el d铆a a d铆a de larga estad铆a. 
  








