# Spring Boot Username and Password Authentication

This project demonstrates a basic Spring Boot application with username and password authentication using Spring Security. It leverages in-memory authentication with an encoded password using `BCryptPasswordEncoder`.

## Features
- In-memory user authentication
- Spring Security configuration for username/password login
- BCrypt password encoding for security
- Conditional bean configuration with `@ConditionalOnMissingBean`
- Custom authentication event publisher

## Project Setup

### Prerequisites
- JDK 8 or higher
- Maven or Gradle for building the project
- Spring Boot 2.x (or compatible)

### Dependencies
The project uses the following dependencies:
- Spring Boot Starter Web
- Spring Security
- Spring Boot Starter Test (for testing)

### How to Run the Project

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/gauravvishalgv/spring-security-user-password.git
   cd spring-security-user-password
   ```

2. Build the project using Maven:

    ```bash
    mvn clean install
    ```
3. Run the Spring Boot application:

    ```bash
    mvn spring-boot:run
    ```
4. The application will start on the port 3333. Access it through your browser or make HTTP requests as required.

### Default User

Username: user
Password: testing (encoded using BCryptPasswordEncoder)

### Accessing the Application

When the application is running, you can test authentication using HTTP requests:

Login URL: /login
Credentials: Use the username user and the password testing.