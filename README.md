# API-REST-SpringBoot-MySQL
Hola, esta es una aplicacion con el marco de trabajo de Spring boot con java y en la base de datos usando MySQL, es un CRUD con las operaciones basicas para guardar registros en la base de datos, a lo largo de la documentacion probaremos la app con Postman.
<br>
<br>
# Configuracion del entorno de trabajo
Para poder ejecutar este proyecto es necesario tener instalado:<br><br>
- MySQL - guia de instalacion: http://gieta.etsisi.upm.es/wp-content/uploads/2020/02/GuiaInstalacion_MySql_Community_8.0.19.pdf <br>
- Maven - guia de instalacion en Windows 10: https://dev.to/vanessa_corredor/instalar-manualmente-maven-en-windows-10-50pb <br>
# Requisitos del proyecto Spring Boot: <br>
- MySQL 8.0 <br>
- Java 11 o superior <br>
# Configura la Base de datos
Es necesario tener una base de datos con el nombre de "api_restful_crud" vacia, ya que el mismo programa creara las tablas.
<br><br>
en la configuracion de la conexion MYSQL los siguientes datos:
- usuario: root
- password:root
# personaliza la configuracion de la base de datos
Para personalizar esto, puedes acceder al archivo application.properties en: src/main/resources y personalizar lo que gustes:

```
spring.jpa.hibernate.ddl-auto=update
spring.datasource.url=jdbc:mysql://localhost:3306/api_restful_crud
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.show-sql: true

spring.mvc.pathmatch.matching-strategy=ant-path-matcher

```
# Ejecuta el servidor local
una vez ya instalado todo lo necesario y ya clonado el proyecto ejecuta el servidor con el siguiente comando:
```
$ mvn spring-boot:run
```
# Añade registros a tu BD

Esto lo puedes hacer directamente en postman, o con un gestor de bases de datos, en este ejemplo usamos MySQL Workbench para agilizar el tiempo.

![Registros de la base de datos](https://github.com/Carranza12/API-REST-SpringBoot-MySQL/blob/master/assets-repo/registros-bd.PNG)

# Probando API con POSTMAN
a continuacion probaremos todos los metodos HTTP de nuestra API.

# GET: Listar todos los clientes
![Registros de la base de datos](https://github.com/Carranza12/API-REST-SpringBoot-MySQL/blob/master/assets-repo/registros-bd.PNG)

# GET: listar un cliente por su id

# POST: Guardar un cliente

# PUT: Actualizar los datos de un cliente

# DELETE: Eliminar un cliente de la BD


