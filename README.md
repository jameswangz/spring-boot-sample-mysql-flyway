# spring-boot-sample-mysql-flyway

spring-boot-sample of JPA/mysql with Flyway migration.

To run it,  first create database on localhost:3306

~~~
create database db_example; -- Create the new database
create user 'springuser'@'localhost' identified by 'ThePassword'; -- Creates the user
grant all on db_example.* to 'springuser'@'localhost'; -- Gives all the privileges to the new user on the newly created database
~~~

Then start the application

~~~
mvn spring-boot:run
~~~

use the following command to create a new model object

~~~
curl "http://localhost:8080/demo/add?name=b&email=b@b.com"
~~~

use the following command to query model objects

~~~
curl "http://localhost:8080/demo/all"
~~~
