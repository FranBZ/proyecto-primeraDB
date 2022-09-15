# Proyecto: Nuestra Primera Base de Datos

## Consigna: 
Tomando como base las clases Contenedor en memoria y en archivos, desarrollar un nuevo 
contenedor con idénticos métodos pero que funcione sobre bases de datos, utilizando Knex para
la conexión. Esta clase debe recibir en su constructor el objeto de configuración de Knex
y el nombre de la tabla sobre la cual trabajará. Luego, modificar el desafío entregable 
de la clase 11 ”Chat con Websocket”, y:
- cambiar la persistencia de los mensajes de filesystem a base de datos SQLite3.
- cambiar la persistencia de los productos de memoria a base de datos MariaDB.
Desarrollar también un script que utilizando knex cree las tablas necesarias para la persistencia en
cuestión (tabla mensajes en sqlite3 y tabla productos en mariaDb).

# Notas:
- Definir una carpeta DB para almacenar la base datos SQLite3 llamada ecommerce

<sup>Formato de entrega: link a un repositorio en Github con los tres proyectos en
carpetas separadas. No incluir los node_modules.</sup>

# Como ejecutar el proyecto
### En tu pc
- Antes que nada debes tener instalado en tu pc node.js
- Debes clonar el repositorio
- Abrir una terminal y en ella dirigirte a la carpeta con el nombre del proyecto
- En la raiz del proyecto debes crear un archivo con el nombre ``` .env ``` y configurarlo con sus respectivos datos:
    ```
    HOST=
    USER=
    PASSWORD=
    DATABASE=
    ```
- Ejecutar el comando ``` npm install ```
- Ejecutar el comando ``` npm run createTables ``` para crear las tablas necesarias, cancelar la ejecucion con ctrl + C
- Una vez finalizado el punto anterior, ejecutar el comando ``` npm run start ```
- Dirigirce al siguiente [Link](http://localhost:8080/productos) para probar la app