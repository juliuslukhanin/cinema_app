# :movie_camera: Cinema App :movie_camera:
# Project description
A simple application that simulates a cinema's ticket-reservation system. The project is based on the Spring framework 
and supports registration, authentication based on roles, adding tickets to the shopping cart and basic CRUD operations

Endpoints:
<pre>
[POST][ADMIN,USER] /register - registers a new user
[POST][ADMIN]      /cinema-halls - creates a new cinema hall
[GET][ADMIN,USER]  /cinema-halls - returns all cinema halls
[POST][ADMIN]      /movies - creates a new movie
[GET][ADMIN,USER]  /movies - returns all movies
[POST][ADMIN]      /movie-sessions - creates a new movie session
[GET][ADMIN,USER]  /movie-sessions/available - returns all available movie sessions for the selected movie
[PUT][ADMIN]       /movie-sessions/{id} - updates a movie session
[DELETE][ADMIN]    /movie-sessions/{id} - deletes a movie session
[POST][USER]       /orders/complete - completes an order
[GET][USER]        /orders - returns order history of user
[PUT][USER]        /shopping-carts/movie-sessions - adds a movie session to shopping cart
[GET][USER]        /shopping-carts/by-user - returns shopping cart of logged user
[GET][ADMIN]       /users/by-email - returns user by email
</pre>

### Project based on 3-layer architecture:
1. Presentation layer
2. Business layer
3. Data layer

### Database structure
![](Hibernate_Cinema_Uml.png)

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
