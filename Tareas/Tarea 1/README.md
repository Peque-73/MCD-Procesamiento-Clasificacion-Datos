# Maestria en ciencia de datos | Procesamiento y clasificación de datos
## Alvaro Pequeño Mondragón

[Código de la tarea](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%201/Tarea_1_Alvaro_Peque%C3%B1o.ipynb)

Para la tarea 1 de esta materia se utilizó un conjunto de datos que contiene los textos extraidos de documentos relacionados a la industria de la iluminación, una pregunta de este conjunto de datos es ver si es posible clasificar los documentos en hojas de especificación y "otros".

Lo primero que se hizo fue obtener los 10 bigramas que mas aparecen en cada una de las clases y se pueden ver a continuación:

![Spec_bigrams](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%201/Spec_bigrams.png)
![Others_bigrams](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%201/Others_bigrams.png)

Se puede observar que entre lso 2 tipos de documentos se comparten 2 bigramas que son "Subject change" y "rights reserved", los demas bigramas son diferentes en cada una de las clases donde en la clase de hojas de especificación podemos observar bigramas relacionados a especificaciones técnicas de las luminarias, mientras que en los otros los bigramas son relacionados a cosas especificas de la marca de las luminarias como lo son direcciones y telefonos por lo que podemos deducir que en esta clase tenemos muchos documentos de la misma compañía.

Por ultimo se graficó la cantidad de palabras que aparecen en los documentos y esta separado por la clase del documento para observar si la cantidad de texto en un documento es un indicador de la clase a la que pertenece:

![Word_count](https://github.com/Peque-73/MCD-Procesamiento-Clasificacion-Datos/blob/main/Tareas/Tarea%201/Word_count.png)

En la grafica anterior se puede observar que los documentos de la clase otros por lo general tiende a tener un numero de palabras bajo a comparación de las hojas de especificación, mientras que las hojas de especificación tienden a tener un gran numero de palabras, por lo general sobrepasando las 2000 palabras por documento.
