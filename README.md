# Proyecto

Por temas de tiempo, usé la base de datos sakila de MYSQL. La base de datos de ejemplo de Sakila está diseñada para representar una tienda de alquiler de DVD. La base de datos de muestra de Sakila todavía toma prestados nombres de películas y actores de la base de datos de muestra de Dell.

1. Descargar la base de datos desde: https://downloads.mysql.com/docs/sakila-db.zip. Donde se obtiene una carpeta comprimida con dos archivos llamados "sakila-data.sql" y "sakila.schema.sql".
   
2. Una vez en MYSQL WORKBENCH, abrir el archivo "sakila.schema.sql" (el cual creará la base de datos y las tablas) y ejecutarlo.
   
3. Ahí mismo en MYSQL abrir el archivo "sakila-data.sql" (el cual llenara las tablas) y ejecutarlo.
   
4. En MYSQL nos dirijimos a la sección de información de session, donde vamos a obtener:
   [informacion.jpg](https://raw.githubusercontent.com/Cath2312/proyecto/main/proyecto/informacion.jpg)
   
5. Descargar python y correr lo siguiente (tomando en cuenta la información que obtuvimos en MYSQL):
    import mysql.connector
   
    configuracion_db = {'user': 'root','password': '101118','host': '127.0.0.1','database': 'sakila'}
   
    try:
   
    conexion = mysql.connector.connect(**configuracion_db)
   
    print("Conexión exitosa a la base de datos")
   
    except mysql.connector.Error as error:
   
    print(f"Error al conectar a la base de datos: {error}"

 6. Ahora en cmd de windows escribimos "Jupyter Notebook" y nos llevara a una ventana de google.

 7. En la ventana nos vamos a "New" -> Python3.

 8. Una vez ahí volvemos a correr el punto 5 en una celda.

 9. Desde ahi podemos trabajar con nuestra base de datos desde python usando nuestra base de datos, como por ejemplo si 
    corremos:

    cursor = conexion.cursor()

    cursor.execute("SELECT * FROM actor")

    resultado = cursor.fetchall()

    for fila in resultado:

      print(fila)

    vamos a obtener:
    
 11. Y asi podemos seguir trabajando en la base de datos desde jupyter:

