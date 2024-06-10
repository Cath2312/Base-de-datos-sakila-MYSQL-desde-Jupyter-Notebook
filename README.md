# Proyecto

Por temas de tiempo, usé la base de datos sakila de MYSQL. La base de datos de ejemplo de Sakila está diseñada para representar una tienda de alquiler de DVD. La base de datos de muestra de Sakila todavía toma prestados nombres de películas y actores de la base de datos de muestra de Dell.

1. Descargar la base de datos desde: https://downloads.mysql.com/docs/sakila-db.zip. Donde se obtiene una carpeta comprimida con dos archivos llamados "sakila-data.sql" y "sakila.schema.sql".
2. Una vez en MYSQL WORKBENCH, abrir el archivo "sakila.schema.sql" (el cual creará la base de datos y las tablas) y ejecutarlo.
3. Ahí mismo en MYSQL abrir el archivo "sakila-data.sql" (el cual llenara las tablas) y ejecutarlo.
4. En MYSQL nos dirijimos a la sección de información de session, donde vamos a obtener:

5. Descargar python y correr lo siguiente:
    import mysql.connector
    configuracion_db = {'user': 'root','password': '101118','host': '127.0.0.1','database': 'sakila'}
    try:
    conexion = mysql.connector.connect(**configuracion_db)
    print("Conexión exitosa a la base de datos")
    except mysql.connector.Error as error:
    print(f"Error al conectar a la base de datos: {error}" 

