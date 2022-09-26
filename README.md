# :oncoming_taxi: Taxi-service :oncoming_taxi:

>Web-application that simulates the work of a taxi service.
Supports authentication, registration and other CRUD operations.


## :pushpin: Content

- [How to start using](https://github.com/ira0807/taxi-service#clipboard-how-to-start-using)
- [Project structure](https://github.com/ira0807/taxi-service#chains-project-structure)
- [Features](https://github.com/ira0807/taxi-service#vibration_mode-features)
- [Technologies](https://github.com/ira0807/taxi-service#books-technologies)


## 	:clipboard: How to start using

>It is recommended to follow the following instructions to run:

1. Fork this repositories
2. Copy link of project
3. Open new project from Version Control and paste this link
4. Edit ConnectionUtil class - write your own data:
```bash
    private static final String URL = "YOUR DATABASE URL";
    private static final String USERNAME = "YOUR USERNAME";
    private static final String PASSWORD = "YOUR PASSWORD";
    private static final String JDBC_DRIVER = "YOUR DRIVER";
```
Example:
```bash
    private static final String URL =
          "jdbc:mysql://localhost:3306/taxi?useUnicode=true&serverTimezone=UTC";
    private static final String USERNAME = "user";
    private static final String PASSWORD = "12345678";
    private static final String JDBC_DRIVER = "com.mysql.cj.jdbc.Driver";
```
5. Create new tables in your database for correct connection, using data from the file `init_db.sql` in `resources` directory
6. Install [Tomcat](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
7. Configure Tomcat server in your IDEA
8. Run project


##  :chains: Project structure
>The project has an N-Tier Architecture:

- Controller - allows the user to work with this application through browser
- Service - is responsible for processing the data received from the DAO level
- DAO - is responsible for communicating with the database


## :vibration_mode: Features

- Log in/out
- Register a new driver
- Create, update, delete car
- Create, update, delete manufacturer
- Create, update, delete driver 
- Add driver to car
- Display list of all cars, manufacturers, drivers, cars of current driver


## :books: Technologies

- [Java 17](https://www.oracle.com/java/technologies/downloads/)
- [Maven](https://maven.apache.org/download.cgi)
- [MySQL](https://dev.mysql.com/downloads/installer/)
- [JDBC](https://www.oracle.com/database/technologies/appdev/jdbc-downloads.html)
- [Tomcat](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
