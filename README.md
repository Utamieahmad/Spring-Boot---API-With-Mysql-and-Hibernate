## 1. Requirements

1. Java - 1.8.x

2. Maven - 3.x.x

3. Mysql - 5.x.x

**2. Create Mysql database**

create database notes_app

**3. Change mysql username and password as per your installation**

+ open `src/main/resources/application.properties`

+ change `spring.datasource.username` and `spring.datasource.password` as per your mysql installation

**4. Build and run the app using maven**

mvn package
java -jar target/easy-notes-1.0.0.jar

Alternatively, you can run the app without packaging it using -
mvn spring-boot:run

The app will start running at <http://localhost:8080>.

## 5. Explore Rest APIs

The app defines following CRUD APIs.

    GET /api/notes
    
    POST /api/notes
    
    GET /api/notes/{noteId}
    
    PUT /api/notes/{noteId}
    
    DELETE /api/notes/{noteId}

You can test them using postman or any other rest client.
