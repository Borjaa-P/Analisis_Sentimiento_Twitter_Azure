# Analisis_Sentimiento_de_Twitter_con_Azure

En este repositorio, realizamos un análisis de los sentimientos en twitter,usando como referencia un hashtag. Para ello, hemos elegido un programa de máxima audiencia y vamos a monitorizar el Hashtag que utiliza durante su emisión.
Lo primero que haremos es descargarnos los tweets, en esta ocasión utilizaremos Python para consumir la Api de Twitter a travás de la librería  **Tweepy**. Este proceso está reflejado en el Script de "Descargar_Tweet".

Una vez tenemos los tweets descargados, utilizamos la plataforma de **Microsoft Azure**, concretamente el servicio de **Azure Cognitive Services** para poder clasificarlos por sentimiento. Este proceso  está reflejado en el Script de "API Azure". 

Ya que este servicio en su modalidad gratuita tiene bastantes restricciones, una vez tengamos un numero adecuado de tweet clasificados, pasamos a  realizar nuestro propio modelo de machine learning. Para ello, haremos uso del servicio de Azure **Machine Learning Studio**, comenzamos realizando un análisis de nuestros datos para obtener el algoritmo de clasificación más adecuado, una vez dispongamos de esta información, creamos un modelo en Azure que lo entrenaremos con dicho algoritmo. Finalmente, descargarnos el modelo para utilizarlo, de esta manera podremos reducir el coste y disponer de este modelo siempre que queramos.

Ya con todos lo tweets clasificados, realizaremos una serie de modificaciones para obtener un DataFrame centrado en los personajes del programa. Este proceso está reflejado en el Script de ‘Concursantes’.

Una vez finalizado todos los procesos, obtenems como resultado dos DataFrame:

1. En el encontramos toda la información relacionada con los tweets.

2. En el encontramos toda la información clasificada por concursante.

Para concluir este proceso, vamos a volcar toda esta información en una herramienta de visualización, en este caso concreto yo he decido utilizar  **Power BI**. 
Aquí adjunto imágenes de alguno de los Dashboard creados para analizar en profundidad la información obtenida.


-Informes PowerBI
 
![Cargando imagen ](https://github.com/Borjaa-P/Analisis_Sentimiento_Twitter_Azure/blob/main/image.png?raw=true)
