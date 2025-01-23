# Tarea 2 Procesamiento y clasificación de datos
## Alvaro Pequeño Mondragón 1726520


# Analisis de sentimientos en textos de goles anotados v.s goles no anotados

## Objetivo
Se tiene una base de datos con textos de eventos de partidos de futbol, de todos los tipos de eventos y jugadas que pueden ocurrir en un juego se decidió analizar los tiros a gol y se dividieron los datos entre aquellos tiros que fueron gol y los que no para así poder ver si en la redacción de los portales deportivos hay una diferencia a la hora de escribir estos textos.

## Analisis de sentimientos
Para el analisis de sentimientos se utilizó la libreria de nltk para hacer la parte del pre procesado y para la parte del score del sentimiento se utilizo nltk haciendo uso de vader. Una vez realizado el analisis de sentimientos a los textos se obtuvieron las siguientes graficas:

En esta primer grafica podemos observar que para los textos de goles anotados en su mayoria con 68% son neutrales mientras que con 22% son positivos y el 10% restante son negativos:

![Sentimientos_goles_anotados](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Sentimientos_goles_anotados.png)

En la segunda grafica podemos ver los sentimientos en los tiros que no fueron goles, donde se observa que el 68% de los textos son negativos el 30% positivos y el 2% neutrales, lo que hace sentido ya que un tiro fallado se puede interpretar como algo malo:

![Sentimientos_goles_no_anotados](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Sentimientos_goles_no_anotados.png)

Por ultimo podemos ver la distrubución de los scores de los textos en ambos casos con los siguientes histogramas:

![Hist_goles_anotados](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Hist_goles_anotados.png)

![Hist_goles_no_anotados](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Hist_goles_no_anotados.png)

Para finalizar se decidió checar un poco mas a fondo los textos correspondientes a los goles para ver si hay algun tipo de sesgo donde a ciertos equipos tengan textos mas positivos que otros por lo que a continuación se muestran los equipos que tienen una puntuacion mucho mas positiva:

![Top_10_equipos_positivos](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Top_10_equipos_positivos.png)

Por ultimo se muestran los 10 equipos con los textos mas negativos:

![Top_10_equipos_negativos](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Top_10_equipos_negativos.png)

## Conclusiones
Me gustaria centrar la conclusion en el analisis de los equipos con un promedio de score en los textos positivos y negativos. En la grafica de los equipos más positivos se pueden observar que hay 4 equipos que sobresalen y me llama la atencion el 4to equipo que se llama Nice, este es un equipo francés y lleva el nombre de una ciudad pero en ingles Nice es una palabra muy positiva por lo que los textos al decir "Gol de Nice" se clasifican como muy positivos aunque en contexto las palabras no necesariamente signifique algo bueno. Es posible que suceda algo similar con los otros 3 equipos, puede que en el proceso de stemming o lemmatizing la raiz que nos queda a partir de los nombres de los equipos sea una raiz asociada a algo muy positivo.

En el caso de los equipos negativos ocurre algo similar al de los equipos positivos pero con el sentimiento contrario ya que se puede observar que hay un equipo que sobre sale de los demas el cual es el Angers, este equipo tambien es francés y lleva el nombre de una ciudad pero en este caso en inglés esta palabra Angers es algo negativo por lo que los textos de este equipo se les da un score negativo.

Tomando en cuenta lo anterior creo que cuando se incluyen muchos nombres o palabras extranjeras que puedan tener un significado en el idioma del analisis se deberia de tener un diccionario con el cual eliminar estas palabras del analisis de sentimientos y evitar ruido en los resultados.

[Código de la tarea](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Tarea_2_Alvaro_Peque%C3%B1o.ipynb)
