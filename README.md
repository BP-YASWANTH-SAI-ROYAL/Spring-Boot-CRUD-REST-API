# Spring-Boot-CRUD-REST-API
This is a simple Spring Boot application demonstrating CRUD (Create, Read, Update, Delete) operations using Spring Web, Spring Data JPA, and MySQL.

🚀 Features
Create new employee entries (POST)

Retrieve all or single employee data (GET)

Update employee details (PUT)

Delete employee records (DELETE)

MySQL integration

Spring Boot 3.5.3

Lombok for reducing boilerplate code

RESTful API architecture

springrestapi/
│
├── src/main/java/in/royal/springrestapi/
│   ├── controller/         # REST controllers
│   ├── model/              # JPA entities
│   ├── repository/         # Spring Data JPA repositories
│   └── service/            # Service layer (business logic)
│
├── src/main/resources/
│   └── application.properties  # DB config
│
├── pom.xml                 # Maven build config
├── HELP.md                 # Spring initial documentation
└── README.md               # Project guide (this file)




🛠️ Setup Instructions
Prerequisites
Java 21

Maven

MySQL database

MySQL DB Setup
Create a database in MySQL:

sql
Copy
Edit
CREATE DATABASE employee_db;
application.properties (example)
properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/employee_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Run the app
bash
Copy
Edit
# Maven build
mvn clean install

# Run Spring Boot app
mvn spring-boot:run
📦 Build and Package
bash
Copy
Edit
mvn package
This will generate a JAR file inside the target/ directory.

🧑‍💻 Developer Notes
Lombok is used for reducing boilerplate code in models (@Getter, @Setter, @NoArgsConstructor, etc.).

Swagger can be integrated for API documentation (optional).

You can extend this project to include:

Validation (@Valid)

Pagination and Sorting

Unit and Integration Tests
