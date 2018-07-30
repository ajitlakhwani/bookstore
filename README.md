### Features

- Bookstore application with save, delete and search capabilities

##### Technologies

- Java 8
- Spring Boot
- Gradle
- JAX-RS Microservices
- JUnit and JBehave
- Angular CLI

                    
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
