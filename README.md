# Java EE Application with PostgreSQL

A simple Java EE application that connects to a PostgreSQL database. It demonstrates how to configure a Java EE servlet to interact with a PostgreSQL database, and provides the option to run the application locally or using Docker.

## Features

- Java EE-based application
- PostgreSQL integration
- Docker support

---

## Requirements

- Java JDK 21+
- Apache Maven
- PostgreSQL (if running locally)
- Docker and Docker Compose (if running in Docker)

---

## Getting Started

### Running in Docker
```bash
  docker-compose up --build
```
### Running Locally

Follow these steps to run the application on your local machine without Docker:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/thealexcesar/music-java-ee.git
   cd music-java-ee
   ```
2. Install Dependencies: Make sure you have Maven installed, then run:
```bash
  mvn clean install
```
3. Set Up PostgreSQL: You need a PostgreSQL instance running on your local machine.

- In your PostgreSQL create a database named spotify.
- Use the following default credentials:
```bash
  Username: your_username
  Password: your_password
  Database: spotfy
```

4. Run the Application:
- Package the application using Maven:
```bash
  mvn package
```

5. http://localhost:8080/my-javaee-app/dbtest

- Deploy the generated WAR file to a local Tomcat instance, or alternatively run it directly with:
5. Deploy the generated WAR file to a local Tomcat instance, or alternatively run it directly with:
