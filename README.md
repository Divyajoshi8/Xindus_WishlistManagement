# Xindus_WishlistManagement

Xindus Assignment: Streamlined Wishlist Management Backend

Welcome to the Xindus Assignment repository! This backend application empowers e-commerce platforms with efficient wishlist management. Crafted on the robust foundation of Spring Boot, Spring Security (leveraging JWT authentication), and Spring Data JPA, this application ensures a secure and seamless experience for users.

# Features

User Authentication: Immerse yourself in a secure environment with a seamless signup and login process, fortified by Spring Security and JWT authentication.
Wishlist Management: Unleash the power of RESTful API endpoints designed for effortless wishlist management. Seamlessly create and delete wishlist items with the provided endpoints.
Database Integration: Forge connections with a relational database through Spring Data JPA. Efficiently store user information and wishlist items for a dynamic and responsive experience.
Setup and Usage:

# Prerequisites           
* Java Development Kit (JDK) version 8 or higher
* Maven


# Installation
* Step 1: Clone the repository to your local machine:
git clone https://github.com/name/your_repository

* Step2:- Navigate to the project directory:
cd XindusWishlistManagement

* Step3:- Build the project using Maven:
mvn clean install

 # Configuration
* Step 1: Database Configuration:

1. Open the src/main/resources/application.properties file.
2. Customize your database connection settings:
   spring.datasource.url=jdbc:mysql://localhost:3306/wishlistmanagement
   spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
   spring.datasource.username=root
   spring.datasource.password=root

* Step 2 : Spring Security Configuration:
1. Customize security settings, such as JWT token expiration time and secret key, in the SecurityConfig.java file.

2. Running the Application:

_Run the application using Maven_
- mvn spring-boot:run

  The application will start on the default port 8080.

# API Usage:

* Sign Up:

1. Open Postman or any HTTP client application.
2. Send a POST request to http://localhost:8080/auth/register with a JSON body containing user details:

   - {
  "firstName": "example_firstname",
  "lastName": "example_lastname",
  "email": "example_email",
  "password": "example_password"
}

* Login:

1. Send a POST request to http://localhost:8080/auth/login with a JSON body containing user credentials:

- {
  "email": "example_email",
  "password": "example_password"
}

Note: Save the JWT token received in the response.

# Accessing Other APIs:

 To access other APIs requiring authentication, include the JWT token in the Authorization header of your requests:

* In Postman, set the Authorization type to "Bearer Token" and paste the JWT token obtained during login.
Endpoints for Other API Functionalities:

* Wishlist Management: http://localhost:8080/api/wishlists
* Products: http://localhost:8080/api/products
Thank you for diving into the Xindus Assignment backend repository! We trust this documentation offers a clear roadmap for setting up, configuring, and utilizing the application. Happy coding!




