# sysderecommyclust
Entregable 3 del Curso de Data Science de ICARO. Sistema de Recomendación y Clustering.

Sistema de Recomendación:

La idea consiste en crear un modelo de recomendacion. Pueden descargar los archivos desde el siguiente link:
https://drive.google.com/drive/folders/1F58VdEmIUakN7dOvaLeEmd5xCRrSJgB6?usp=sharing

El primer paso consiste en lograr leer los archivos desde el drive y armar los 2 datasets, el de entrenamiento y el de validacion.

Se pide ademas, crear un 3er conjunto de testeo donde deberan extraer de los primeros 2 un sample y no utilizar estos datos para entrenar. Es decir, del conjunto total de datos, armar 3 dfs, training, test y validation.

Desarrollar un recomendador. El recomendador debe ser capaz de generar recomendaciones para TODOS los usuarios (incluyendo los cold start que no tengan visualizaciones en el set de train). Generar 20 recomendaciones por usuario.

Las recomendaciones tienen que ser para cada account_id y hay que recomendar content_id.

Los contenidos que recomienden, no tienen que haber sido vistos previamente por los usuarios (filtrar). Se acepta solamente que se recomiende este caso si el usuario vio el contenido solamente 1 vez y el mismo posee un rating que se encuentre en el ultimo decil.

Evaluarlo con MAP.

Se valora la originalidad en el codigo.

Recomendaciones:

Al momento de leer los datos, los archivos llamados "base" forman el conjunto de training y los "test" el de test.
Quedarse con las columnas user_id; item_id; raiting; ts
Comenzar con algo simple
Cuando el modelo ya este funcionando, mejorarlo e ir cubriendo los distintos requisitos.
También pueden probar con un dataframe mayor: https://grouplens.org/datasets/movielens/

Clustering:

La idea principal es que primero consigan el dataset con el cual deberán trabajar. Una vez que tengan su dataset, la idea es que apliquen como mínimo los 2 modelos de clustering que vimos, el de K-Means y DBScan. Es necesario que incluyan una optimizacion de hiperparametros (según las metricas de Inercia y Silueta). Cuando ya tengan segmentados los datos, tienen que analizar y encontrar las caracteristicas de cada uno.
