¿SE PUEDE PREDECIR UN GOL MEDIANTE UN REMATE?

El objetivo de este trabajo es desarrollar un modelo de clasificación para predecir la probabilidad de gol a partir de remates registrados en partidos de fútbol. Utilizando un conjunto de datos de eventos de remates, se analiza información relevante como la distancia al arco, el ángulo del remate, el tipo de remate y la posición del arquero. Logramos limpiar y explorar el conjunto de datos que brinda statsbomb, identificando variables claves que servirán de base para el desarrollo del modelo predictivo en las siguientes etapas.

📝 Pasos para reproducir el proyecto

📁 Ir a datastatsbomb/

En esta carpeta normalmente se realiza la descarga de los datos desde la API de StatsBomb.

En este caso, ya contamos con los archivos necesarios descargados. https://drive.google.com/file/d/1WI6noUvvGM_VLIvOkOoYZc659MAdjLYC/view?usp=sharing

Por lo tanto, dirigirse directamente a la sección (CAJA nro 6) donde se carga el archivo eventosremates.csv y comenzar con el proceso de limpieza.

🧹 Limpiar el dataset En el archivo correspondiente dentro de datastatsbomb/, realizando:

Filtrado de eventos específicos relacionados a remates.

Se unió el conjunto de datos de información de jugadores, por lo tanto se necesita este conjunto de datos para continuar https://drive.google.com/file/d/1mKUpb_vQkv2qqRmLay6ROjIxHISIrrI-/view?usp=sharing Eliminación de columnas irrelevantes.

Creación de variables.

El resultado de esta limpieza será utilizado en el siguiente paso.

Conjunto de datos final -> https://drive.google.com/file/d/1KaEDWdK1_jBYKSeGwM0KplWUkpx-jMd8/view?usp=sharing

📂 Ir a dataremates/

En esta carpeta ya se trabaja con el conjunto de datos limpio.

Nos divertimos un poco con los gráficos para entender mejor los datos, explorando cómo se distribuyen los remates y qué variables podrían influir en el resultado del disparo.

📁 Ir a modeloremates/ En esta carpeta se encuentra el modelo de regresión logística.

Se entrena el modelo utilizando el conjunto de datos generado.

Se evalúa el rendimiento del modelo y se muestran métricas.
