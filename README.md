# User Registration and Login System

This project is a simple User Registration and Login System built using PHP, MySQL, HTML, CSS, and JavaScript. It allows users to register, log in, and view a personalized homepage.

## Features

- User registration with first name, last name, email, and password.
- User login functionality.
- Personalized homepage displaying the user's name after logging in.
- Logout functionality.

## Technologies Used

- PHP
- MySQL
- HTML
- CSS
- JavaScript

## Project Structure

/project-directory
│
├── index.php # Main registration and login page
├── homepage.php # User's homepage after login
├── connect.php # Database connection file
├── logout.php # Logout functionality
├── style.css # Styles for the application
└── script.js # JavaScript for handling form display

## Prerequisites

- A local server environment (e.g., XAMPP, WAMP, MAMP) with PHP and MySQL support.
- A web browser to access the application.

## Setup Instructions

1. **Clone or Download the Repository**:
   - Clone this repository or download the project files to your local machine.

2. **Set Up Your Environment**:
   - Install a local server environment (XAMPP, WAMP, or MAMP).

3. **Create a Database**:
   - Open phpMyAdmin (usually accessible at `http://localhost/phpmyadmin`).
   - Create a new database named `login`.
   - Create a table named `users` with the following SQL command:
     ```sql
     CREATE TABLE users (
         id INT AUTO_INCREMENT PRIMARY KEY,
         firstName VARCHAR(50) NOT NULL,
         lastName VARCHAR(50) NOT NULL,
         email VARCHAR(100) NOT NULL UNIQUE,
         password VARCHAR(255) NOT NULL
     );
     ```

4. **Place Your Files**:
   - Copy the project files (`index.php`, `homepage.php`, `connect.php`, `logout.php`, `style.css`, `script.js`) into the `htdocs` directory (or equivalent) of your local server.

5. **Configure Database Connection**:
   - Open `connect.php` and ensure the database connection details are correct. The default username for XAMPP is `root` and the password is empty.

6. **Start Your Server**:
 - Start the Apache and MySQL services from your server control panel (like XAMPP Control Panel).

7. **Access the Application**:
   - Open a web browser and navigate to `http://localhost/index.php` to access the registration and login page.

## Usage

1. **Register a New User**:
   - Fill in the registration form with your first name, last name, email, and password, then click "Sign Up".

2. **Log In**:
   - After registering, you can log in using your email and password.

3. **View Homepage**:
   - Upon successful login, you will be redirected to your personalized homepage displaying your name.

4. **Logout**:
   - Click the "Logout" link to end your session.

## Security Note

- Ensure to implement password hashing when storing passwords in the database for security. You can modify the registration logic in `register.php` (not provided) to include password hashing using `password_hash()`.

## License

This project is open-source and available for use and modification. Please feel free to contribute or suggest improvements.

## Acknowledgments

- Thanks to the open-source community for providing the tools and resources to build this project.


# login-form-with-database-connection
you can watch the full tutorial on my youtube channel 
https://www.youtube.com/@francis_tech
