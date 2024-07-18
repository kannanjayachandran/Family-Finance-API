# Family-Finance-API

A RESTful API for managing digital debit cards within a family, built using Spring Boot. 
The application allows families to create, update, retrieve, and delete cash cards, ensuring secure 
access and management.

## Features
- **CRUD** Operations: Create, read, update, and delete cash cards.

- **Authentication** & **Authorization**: Secure endpoints using Spring Security.

- **Data Persistence**: Store and retrieve data using Spring Data JDBC.

- **Pagination & Sorting**: Efficiently handle lists of cash cards.

- **Testing**: Implement test-driven development for reliable code.

## Technologies Used

- **Spring Boot**: Framework for building the API.

- **Spring Security**: Secures the application.

- **Spring Data JDBC**: Manages database interactions.

- **JUnit**: Framework for testing.

## Prerequisites
- Java 8 or higher

- Maven or Gradle

- A database (e.g., H2, MySQL, PostgreSQL) {H2 is used here}

## Getting Started

1. Clone the repository:

```bash
git clone https://github.com/kannanjayachandran/Family-Finance-API.git

cd Family-Finance-API
``` 

2. Build and run the application:

**Using Maven:**

```bash
mvn clean install
mvn spring-boot:run
```

**Using Gradle:**

```bash
./gradlew build
./gradlew bootRun
```

## Access the API

The API is accessible at `http://localhost:8080/`.

## API Endpoints

### Create a Cash Card

```http
POST http://localhost:8080/cashcards
```

### Retrieve a Cash Cards

```http
GET http://localhost:8080/cashcards/{id}
```

### Updata a Cash Cards

```http
PUT http://localhost:8080/cashcards/{id}
```

### Delete a Cash Cards

```http
DELETE http://localhost:8080/cashcards/{id}
```

### List all Cash Cards

```http
GET http://localhost:8080/cashcards
```

## Security

The API is secured using Spring Security. To access the endpoints, you need to provide a valid 
username and password. 

## Testing

Run the tests using Maven or Gradle:

**Using Maven:**

```bash
mvn test
```

**Using Gradle:**

```bash
./gradlew test
```

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
