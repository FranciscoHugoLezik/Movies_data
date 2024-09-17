Contiene los archivos de datos utilizados en el proyecto llamado Proyecto_Peliculas. Es público. El github de este proyecto es el siguiente:

https://github.com/FranciscoHugoLezik/Proyecto_Peliculas.git

Adentro hay una carpeta llamada credits y un archivo csv llamado 'movies_dataset.csv'. Dentro de carpeta credits hay dos archivos parquet. Uno se llama cast.parquet y el otro se llama crew.parquet. 

Originalmente los datos de los dos archivo parquet estaban en un archivo csv llamado credits.csv. Este archivo supera el maximo de 100 Mb que puede tener un archivo para subirse a GitHub. En otra carpeta, distinta del proyecto, cree una notebook, lo converti en un dataframe y luego lo exporte a un archivo parquet llamado credits.parquet. Pero surgio otro problema, aunque menos grave. GitHub recomienda que los archivos no superen los 50 Mb y credits.parquet lo superaba.

Aunque lo puedo subir a GitHub quiero cumplir con el tamaño recomendado de los archivos. El archivo credits.csv tiene tres columnas: cast, crew y id. Lo dividi en dos dataframes. El primero contiene la columna cast y la columna id. El segundo contiene la columna crew y la columna id. Luego exporte ambos dataframe para convertirlos en archivos parquet. Comparten la misma columna id para que se conserve la relacion.

El otro archivo csv llamado movies_datasets.csv aunque no supera los 50 Mb lo converti al tipo parquet. Lo hice porque para mi queda mas prolijo que todos los archivos sean del mismo tipo.