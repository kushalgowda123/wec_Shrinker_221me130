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
2. Install the required npm packages:

   npm install
3. Set up PostgreSQL:

  Install PostgreSQL and pgAdmin.
  Create a new PostgreSQL database named postgres.
  Update the database connection details in the code to match your setup (host, user, password, port).
  Run the provided SQL queries to set up the required tables:
  users: To store user information (email, password).
  url: To store the long URL, short URL, and the user who created it.
4. Start the server: nodemon index.js
5.Open your browser and visit http://localhost:3000 to access the application.
6.Routes
  Public Routes:
  /: Home page.
  /register: User registration page.
  /login: User login page.
  Protected Routes (Login Required):
  /shorten: URL shortening page.
  /urls: Page to view all shortened URLs by the logged-in user.
