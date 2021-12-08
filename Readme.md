# REST Survey App
**Developer**: Daniil Livitin <br> <br>
**Technical Stack**: 
* Java, Spring Framework, Liquibase, PostgreSQL, Swagger <br>
## How to install project?

<i>In order to install this project locally, proceed with the following steps:</i>
<br>

1) Clone this repository to your machine using command:<br> `git clone https://github.com/Dablup/REST_survey_app.git` <br><br>
2) Then, you need to create a database and specify the path to it in the `application.properties`. <br> Note: Path to `application.properties`: [application.properties](/src/main/resources/application.properties)
```
spring.datasource.url=jdbc:postgresql://localhost:5432/akvelon
spring.datasource.username=postgres
spring.datasource.password=root
```
3) Using the command line, navigate to the root folder of the project and run the command:
```
mvn clean install
``` 
4) After a successful build, you need to run the command:
```
java -jar .target/akvelon-0.0.1-SNAPSHOT.jar

or

java -jar target/akvelon-0.0.1-SNAPSHOT.jar
```

## Important points:
1) To check the documentation of the API, you need to run the project and then follow this link: [Swagger Documentation](http://localhost:8080/swagger-ui/)
<br><br>![image](https://user-images.githubusercontent.com/44948387/145263198-fe02385a-b0d3-44e2-98de-cce28522e063.png)
<br><br>
2) When you start the project it automatically creates needed tables in database. Besides, it inserts some data to db. It is done with the help of [**liquibase**](https://www.liquibase.org/).

3) All tests were passed during building the project.
<br><br>![image](https://user-images.githubusercontent.com/44948387/145263982-70e987d7-bff0-4410-b7b7-b85e5288df30.png)
