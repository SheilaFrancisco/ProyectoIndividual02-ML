# <h1 align=center> **PROYECTO INDIVIDUAL Nº2** </h1>

# <h1 align=center>**`Machine Learning`**</h1>

<hr> 
<br/>
<br/>

El objetivo de este proyecto fue predecir, mediante un modelo de Machine Learning, el precio de inmuebles en Estados Unidos, para lo cual se proporcionaron dos datasets con información sobre diversos inmuebles. 

De los datasets proporcionados, uno se ocuparía para el entrenamiento y el otro para el testeo; el primero de ellos incluía la columna objetivo: `Precio`, con base en la cual se debían catalogar las propiedades en 'low' (0 a 999 dolares), 'medium' (1000 a 1999 dolares) y 'high' (2000 dolares o mayor) y posteriormente realizar una segunda clasificación donde se codificara con 1 a los inmuebles con precios 'low' y con 0 a todo lo que no fuera 'low'.

La primera parte del proyecto consistió en hacer un análisis exploratorio de los datos y así definir las mejores variables para entrenar el modelo. Durante esta exploración del dataset se observó que las descripciones de los inmuebles, contenidas en la columna `'description'`, eran amplias y bien explicadas, por ello se decidió seguir un enfoque orientado al **Procesamiento de Lenguaje Natural** (NLP por sus siglas en inglés). 

Después de seleccionar las variables para el modelo se realizó el pre-procesamiento del texto, removiendo las palabras vacías (stopwords), Url's, entre otros y se realizó la derivación (stemming) de las palabras. Siguiendo con la ingeniería de características, se utilizó el enfoque de **Bolsa de palabras** (bag of words) que consiste en generar un vector que represente todas las palabras del corpus.

Finalmente, se procedió al modelado utilizando como clasificador el modelo de ensamble **Ramdom Forest**. Se eligió este modelo ya que es robusto frente a outliers y ruido, además de que trabaja bien con grandes conjuntos de datos.

Este proceso se puede ver en el archivo *Modelo_Supervisado.ipynb* alojado en este mismo repositorio.
