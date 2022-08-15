# :movie_camera: Cinema App :movie_camera:
# Project description
A simple application that simulates a cinema's ticket-reservation system. The project is based on the Spring framework 
and supports registration, authentication based on roles, adding tickets to the shopping cart and basic CRUD operations

### Project based on 3-layer architecture:
1. Presentation layer
2. Business layer
3. Data layer

### Database structure
![](structure.png)

### Used technologies:
- Java 11
- MySQL 8.0.22
- Spring Core 5.2.2
- Spring MVC 5.2.2
- Spring Security 5.2.2
- Hibernate 5.4.27
- TomCat 9.0.50

### How to run this project:
1. Clone this project
2. Install MySQL and Apache Tomcat 
3. Setup DB parameters in resources/db.properties
4. To inject default roles send GET request to http://localhost:8080/inject
5. And now you can log in as admin with the following data: email — admin@i.ua, password — admin123
