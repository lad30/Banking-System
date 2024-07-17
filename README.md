# Bank-Management-System
The Bank Management System allow you to perform various banking operation including managing accounts, fund transfers, and transactions.

# Prerequisites
- Basic knowledge of Java and the Spring Framework.
- A code editor of your choice (e.g., `VSCode, IntelliJ IDEA, Eclipse`).
- Postman for testing API endpoints.
- A MySQL database.

# Features
- **User Registration:** Users can register by providing their details, such as name, email, address, and phone number.
- **PIN Management:** Users can create and update their PINs for added security.
- **Cash Deposit and Withdrawal:** Users can deposit and withdraw cash from their accounts.
- **Fund Transfer:** Users can transfer funds to other accounts within the system.
- **Transaction History:** Users can view their transaction history.

# Technologies used
- Java Spring Boot Framework
- Spring Security for authentication
- JWT (JSON Web Token) for secure API authentication
- MySQL for data storage
- Hibernate for object-relational mapping
- Maven for project management
- Postman for API testing

# Dependencies
- Spring data jpa
- Spring web
- Spring start validation
- Spring security
- Spring devtools
- Spring starter mail
- Spring starter cache
- Mysql connector
- Jwt
- Jackson

# Installation and Setup
- Configure MySQL: Set up a MySQL database and update the database credentials in application.properties.
- Build and run the project: `mvn spring-boot:run`

# Database configuration
- Add below properties in application.properties
```
server.port=8080
spring.datasource.url=jdbc:mysql://localhost:3306/bankManagement
spring.datasource.username=root
spring.datasource.password=root
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform = org.hibernate.dialect.MySQL5Dialect
spring.jpa.generate-ddl=true
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto = update
spring.main.allow-circular-references=true
server.error.include-message=always
# JWT Configuration
jwt.secret=your-secret-key
jwt.expiration=86400000 # Token expiration time in milliseconds (e.g., 24 hours)
jwt.header=Authorization
jwt.prefix=Bearer
```

# Error Handling
- For error handling I am using global exception handling to throw exceptions.


