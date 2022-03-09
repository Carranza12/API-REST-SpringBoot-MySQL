# API-REST-SpringBoot-MySQL
Hola, esta es una aplicacion con el marco de trabajo de Spring boot con java y en la base de datos usando MySQL, es un CRUD con las operaciones basicas para guardar registros en la base de datos, a lo largo de la documentacion probaremos la app con Postman.
<br>
<br>
# Configuracion del entorno de trabajo
Para poder ejecutar este proyecto es necesario tener instalado:
-MySQL - guia de instalacion: http://gieta.etsisi.upm.es/wp-content/uploads/2020/02/GuiaInstalacion_MySql_Community_8.0.19.pdf
-Maven - guia de instalacion en Windows 10: https://dev.to/vanessa_corredor/instalar-manualmente-maven-en-windows-10-50pb
# Requisitos del proyecto Spring Boot
-MySQL 8.0
-Java 11 o superior
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
#Ejecuta el servidor local
una vez ya instalado todo lo necesario y ya clonado el proyecto ejecuta el servidor con el siguiente comando:

$ mvn spring-boot:run
