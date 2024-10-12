# Shrinker URL Shortener

Shrinker is a URL shortener application that allows users to register, login, and shorten long URLs. The application provides an authentication system using Passport.js, and only authenticated users can shorten URLs and view their own shortened URLs.

## Features

### User Roles:
- **User**: Can register, login, shorten URLs, and view their shortened URLs.

### Core Functionalities:
- **User Registration**: Allows users to create an account with their email and password.
- **User Authentication**: Users can log in using their credentials.
- **URL Shortening**: Authenticated users can shorten URLs and assign a name to each shortened URL.
- **URL Management**: Users can view a list of all URLs they have shortened.

## Technologies Used:
- **Node.js**: Backend server built using Express.js.
- **PostgreSQL**: Database to store user data and shortened URLs.
- **Passport.js**: Authentication middleware for handling user logins.
- **Bcrypt**: For secure password hashing.
- **TinyURL**: API for shortening URLs.
- **EJS**: Templating engine for rendering HTML.

## Installation

### Prerequisites:
- **Node.js**: Make sure Node.js and npm are installed on your system.
- **PostgreSQL**: Ensure PostgreSQL is installed and running.

### Steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/kushalgowda123/wec_Shrinker_221me130.git
   ```

2. Install the required npm packages:
   ```bash
   npm install
   ```

3. Set up PostgreSQL:
   - Install PostgreSQL and pgAdmin.
   - Create a new PostgreSQL database named `postgres`.
   - Update the database connection details in the code to match your setup (host, user, password, port).
   - Run the provided SQL queries to set up the required tables:
     - `users`: To store user information (email, password).
     - `url`: To store the long URL, short URL, and the user who created it.

4. Start the server:
   ```bash
   nodemon index.js
   ```

5. Open your browser and visit `http://localhost:3000` to access the application.

## Routes

### Public Routes:
- `/`: Home page.
- `/register`: User registration page.
- `/login`: User login page.

### Protected Routes (Login Required):
- `/shorten`: URL shortening page.
- `/urls`: Page to view all shortened URLs by the logged-in user.
- 
### screen shot:
Home page-
<img width="1710" alt="Screenshot 2024-10-12 at 11 34 43 PM" src="https://github.com/user-attachments/assets/e19ec8b8-6700-43db-82da-333779998a5a">
Register page--
<img width="1710" alt="Screenshot 2024-10-12 at 11 35 10 PM" src="https://github.com/user-attachments/assets/a2b8caa9-61b7-449f-a5bf-2d75108520de">
Login page--
<img width="1710" alt="Screenshot 2024-10-12 at 11 36 15 PM" src="https://github.com/user-attachments/assets/b532bbd7-2015-465e-b2d7-c26c31c16f94">
Home page--
<img width="1710" alt="Screenshot 2024-10-12 at 11 38 09 PM" src="https://github.com/user-attachments/assets/19b2cf00-4c42-4c69-b523-28dd1a54e809">
storedurls--
<img width="1710" alt="Screenshot 2024-10-12 at 11 39 06 PM" src="https://github.com/user-attachments/assets/df12a318-3845-4d73-9c46-99af73f49391">
