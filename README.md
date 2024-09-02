# spring-drools
[![License](http://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

Minimal [Spring Boot](http://projects.spring.io/spring-boot/) sample app.

Drools decision table implementation in spring boot

## Requirements

For building and running the application you need:

- [JDK 1.8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [Maven 3](https://maven.apache.org)

## Running the application locally

There are several ways to run a Spring Boot application on your local machine. One way is to execute the `main` method in the `com.drools.example.SpringDroolsApplication` class from your IDE.

Alternatively you can use the [Spring Boot Maven plugin](https://docs.spring.io/spring-boot/docs/current/reference/html/build-tool-plugins-maven-plugin.html) like so:

```shell
mvn spring-boot:run
```


## Requests
URL: http://localhost:9091/order
Method: POST
Request body:
```
{
	"name":"Mobile",
	"cardType":"HDFC",
	"price":15000
}
```

Response body:
```
{
    "name": "Mobile",
    "cardType": "HDFC",
    "discount": 10,
    "price": 15000
}
```
