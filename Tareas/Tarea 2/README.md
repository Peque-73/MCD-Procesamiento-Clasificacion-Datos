# Tarea 2 Procesamiento y clasificación de datos
## Alvaro Pequeño Mondragón 1726520


# Analisis de sentimientos en textos de goles anotados v.s goles no anotados

## Objetivo
Se tiene una base de datos con textos de eventos de partidos de futbol, de todos los tipos de eventos y jugadas que pueden ocurrir en un juego se decidió analizar los tiros a gol y se dividieron los datos entre aquellos tiros que fueron gol y los que no para así poder ver si en la redacción de los portales deportivos hay una diferencia a la hora de escribir estos textos.

## Analisis de sentimientos
Para el analisis de sentimientos se utilizó la libreria de nltk para hacer la parte del pre procesado y para la parte del score del sentimiento se utilizo nltk haciendo uso de vader. Una vez realizado el analisis de sentimientos a los textos se obtuvieron las siguientes graficas:

En esta primer grafica podemos observar que para los textos de goles anotados en su mayoria con 68% son neutrales mientras que con 22% son positivos y el 10% restante son negativos:

![Sentimientos_goles_anotados](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%202/Sentimientos_goles_anotados.png)
