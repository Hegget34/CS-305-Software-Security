# Artemis Financial Secure Communication Implementation

## Project Overview
This project implements secure communication protocols for Artemis Financial's web application. The implementation focuses on adding a file verification step using SHA-256 checksum to ensure data integrity, as well as implementing HTTPS to secure data in transit.

## Developer
Trevor Hegge

## Features Implemented
- SHA-256 hash algorithm for secure checksum verification
- Self-signed SSL certificates for secure communication
- HTTPS protocol implementation
- Input validation and secure error handling
- Dependency vulnerability checking

## Project Structure
- `src/main/java/com/snhu/sslserver/SslServerApplication.java`: Main application class
- `src/main/java/com/snhu/sslserver/ServerController.java`: Controller implementing the checksum functionality
- `src/main/resources/application.properties`: Configuration for SSL and server settings
- `keystore.p12`: SSL certificate keystore

## How to Run the Application
1. Ensure Java JDK 8 or higher is installed
2. Navigate to the project directory in a terminal/command prompt
3. Run the application using Maven: ./mvnw spring-boot:run
     or on Windows: mvnw.cmd spring-boot:run
4. Access the secure endpoint at https://localhost:8443/hash

## Security Testing
The project includes dependency check testing to identify vulnerabilities in dependencies. To run the dependency check:

## Required Environment
- Java 8+
- Maven
- Spring Boot 2.2.4

## Note on SSL Certificate
The application uses a self-signed certificate for demonstration purposes. In a production environment, this would be replaced with a certificate from a trusted Certificate Authority.
