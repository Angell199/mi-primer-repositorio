-------Comando para ejecutar Docker con PostgreSQL-------

docker run: Inicia un nuevo contenedor.
--name mi_postgres: Le da un nombre al contenedor.
-e POSTGRES_PASSWORD=yourpassword: Establece la contraseña del usuario postgres.
-p 5432:5432 : Expone el puerto 5432 del contenedor al mismo puerto del host.
-d: Ejecuta el contenedor en segundo plano (modo "detached").
postgres: Es la imagen oficial de PostgreSQL desde Docker Hub.

-------Pasos para configurar DataGrip-------
Crear nueva conexión
Haz clic en "+" > Data Source > PostgreSQL.
En la ventana de configuración, completa los siguientes campos:
--Host: localhost
--Port: 5432
--User: postgres
--Password: yourpassword
--Database: postgres

