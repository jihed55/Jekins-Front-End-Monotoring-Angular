# Final year project : Monitoring platform using Jenkins ecosystem 

## Spring Backend Server Project 
>The project is based on a web server application used as midelware between the client and Jenkins server which uses the following technologies:
-Eclipse Ide 
-Java Jdk 11.0.6
-Spring MVC with Spring Boot and spring Security
-Maven
-Jenkins 
-PostgresSql 
-Jenkins ver. 2.204.2

The architecture of this application is built with the following part:



![](https://i.imgur.com/j0T3aD7.png)



Controller: Implements the processing logic of the web service (Rest Api ), parsing of parameters and validation of in- and outputs.
Service: Implements the business logic and handles the access to the DataAccessObjects.
DataAccessObjects: Interface for the database. Inserts, updates, deletes and reads objects from the database.
DomainObjects: Functional Objects which might be persisted in the database.
Jenkins Communication Module : Rest Api Layer used to communicate with th jenkins server .
Jenkins Server
## :memo: Purpose
This document describes setup guidance for the market Project.

## Setup 
* Configure The App to be runned on 8081 as a Port
* Configure The Jenkins To be running on 8080 as a port (http://localhost:8081)
* configure Postgres Sql to be running on 3306 as a port 

* 1. - [ Note  : You must add these rows to the data base before you run your server :
* INSERT INTO roles(name) VALUES('ROLE_USER');
INSERT INTO roles(name) VALUES('ROLE_MODERATOR');
INSERT INTO roles(name) VALUES('ROLE_ADMIN');
] 

## How to start the app :accept: 
-Build The Project Using Maven From Eclipse
-Run Project From Eclipse
You should be able to starts a webserver on port 80801 (http://localhost:8081) .

## Frontend Dependencies
Move into the project Directory, open cmd in interface folder 
```
cd my-project 
npm install 
ng serve 
```












