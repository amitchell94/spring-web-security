# Spring Web Security
A skeleton project to demo securing a web application using Spring Security.

The web application is a Spring MVC application that secures the page with a login form backed by a fixed list of users.

## Getting Started

You can get started by cloning the project to your local machine:
```
$ git clone https://github.com/amitchell94/spring-web-security.git
```

### Prerequisites

In order to execute this program you will need have the Java JDK installed.

## Running the Application

The application can be run by packaging everything in a single, executable JAR file, driven by a Java `main()` method. Spring's support for embedding the Tomcat servlet container as the HTTP runtime can be used instead of deploying to an external instance.

`src/main/java/hello/Application.java`

```
include::complete/src/main/java/hello/Application.java[]
```

Once the application starts up, point your browser to http://localhost:8080. You should see the home page.


When you click on the link, it attempts to take you to the greeting page at `/hello`. But because that page is secured and you have not yet logged in, it takes you to the login page.

At the login page, sign in as the test user by entering "user" and "password" for the username and password fields, respectively. Once you submit the login form, you are authenticated and then taken to the greeting page.

If you click on the "Sign Out" button, your authentication is revoked, and you are returned to the log in page with a message indicating you are logged out.

## Built With

* [Gradle](https://gradle.com/) - Dependency Management

## Authors

* **Andy Mitchell** - *Initial work* - [GitHub](https://github.com/amitchell94)

## Acknowledgments

* Created using the [Spring Web Security Tutorial](https://spring.io/guides/gs/securing-web/) 
