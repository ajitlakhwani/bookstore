### Features

- Bookstore application with save, delete and search capabilities

**Table of contents**

- [Technologies](#technologies)
- [Details](#details)
    + [Project Structure](#project-structure)
    + [Rest Endpoints](#rest-endpoints)
    + [Bean](#bean)
    + [Testing](#testing)
    + [Git Strategy](#git-strategy)

##### Technologies

- Java 8
- Spring Boot
- Gradle
- JAX-RS Microservices
- JUnit and JBehave
- Liquibase and MySQL
- Angular CLI
<<<<<<< HEAD
"# Team5" 
=======

                    
### Details

###### Project Structure

`Multi module gradle project`
```
+-- bookstore-ui
	+-- build.gradle
+-- bookstore-services
	+-- build.gradle
	+-- src/main/java
	+-- src/main/resources
	+-- src/test/java
+-- build.gradle
+-- settings.gradle
```
###### Rest Endpoints

| Endpoint | Description|
| -------------| ------------------------------ |
| `GET`  book/get | Return a book for specified path param |
| `POST` book/add | Add a book for request payload |
| `DELETE` book/delete | Delete a book for specified path param      |
| `GET` book/search | Search a book with given criteria (Java 8 - Lambda)  |

###### Bean

```java
public class Book {
	private Long id;
	private String name;
	private String code;
	private String price;
	private String authors;
	private String isbn;
	private String publisher;
	private Date publishedOn;
}
```

###### Testing

`90% Test coverage using Junit and JBehave`

###### Git Strategy

```seq
master->dev: work in dev branch
dev-->feature: major feature
feature-->dev: megre
dev-> master: pull request
```

![](https://nvie.com/img/git-model@2x.png)
>>>>>>> ff4e4070c9e4d1e582ff685e159840766a17ff0e
"# Team5" 
