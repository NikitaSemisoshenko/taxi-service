# **Taxi Service**

Simple tool for managing taxi depot.

## How it works

Main functionality of this service is adding cars and drivers to a database and connecting them to each other.

* create driver and add him to the database;
* create manufacturer and add to the database for connecting with car;
* create and add car;

## Structure of project

* _dao layer_ interacts with database;
* _controller layer_ contains http servlets. They are receiving requests and responds to them;
* _service layer_ executes business logic of app;
* _lib package_ contains Injector and annotations. Injector helps us to reach Inversion of Control principle;
* _web.filter package_ contains filters. We use them for such purposes as restricting access for those users who
not exist at database;
* _model package_ contains entities which we interact while the application is running;
* _util package_ contains utilities such as ConnectionUtil. It helps us to connect with database;
* _exception package_ contains custom exceptions;

## Things used for app development

* MySQL;
* Servlet API;
* JDK 11;
* Tomcat 9.0.64;
* Maven;
* JDBC;

## How to start the project 
* create schema and tables using your sql console and data from _src/main/resources/init_db.sql_;
* install Tomcat of 9.x.xx version (**be careful! If Tomcat's version will be 10.x.xx you won't start the app**);
* open ConnectionUtil class at util package. Input your data for connecting with database;.
* configure your Tomcat [see here how](https://www.loom.com/share/1862b4eca21d469b938ca1928f704f36);
* press "Start" button on the top or press Shift + F10;
