# Password Reset Flow - Frontend

A React-based web application that supports secure user authentication and password reset functionality. Designed with **Bootstrap** for responsive UI, the app allows users to register, log in, and reset their passwords as needed. It connects to a Node.js backend with RESTful API endpoints to handle authentication and password management.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Application Pages and Components](#application-pages-and-components)
  - [Login Page](#login-page)
  - [Register Page](#register-page)
  - [Forgot Password Page](#forgot-password-page)
  - [Reset Password Page](#reset-password-page)
- [API Endpoints](#api-endpoints)
- [Setup Instructions](#setup-instructions)
- [License](#license)

---

## Project Overview

This project is a user authentication frontend application where users can securely sign up, log in, and manage password resets through an email link. The app leverages a responsive design and API integration with a Node.js backend, creating a seamless and secure user experience across devices.

---

## Features

- **User Registration & Authentication**: Securely register and log in with validation.
- **Password Reset Flow**: Users can request a password reset via email and set a new password.
- **Responsive UI**: Designed with **Bootstrap** for a smooth mobile and desktop experience.
- **API Communication**: Connects to a backend with endpoints for registration, login, and password reset.

---

## Technology Stack

- **React**: Frontend library for building dynamic user interfaces.
- **Bootstrap**: CSS framework for a responsive and modern UI.
- **Axios**: HTTP client for seamless API communication.
- **React Router**: Handles application routing and navigation.

---

## Application Pages and Components

### Login Page

- **Path**: `/login`
- **Description**: Allows users to authenticate with their email and password.
- **Component**: `Login.js`

### Register Page

- **Path**: `/register`
- **Description**: Provides a form for new users to create an account.
- **Component**: `Register.js`

### Forgot Password Page

- **Path**: `/forgot-password`
- **Description**: Users can enter their email to receive a password reset link.
- **Component**: `ForgotPassword.js`

### Reset Password Page

- **Path**: `/reset-password`
- **Description**: Allows users to set a new password after accessing the reset link in their email.
- **Component**: `ResetPassword.js`

---

## API Endpoints

The frontend interacts with a backend API for user management. The following endpoints are required:

- **POST** `/auth/register`: Registers a new user.
- **POST** `/auth/login`: Authenticates a user and returns a JWT token.
- **POST** `/auth/requestPasswordReset`: Sends a password reset link to the user's email.
- **POST** `/auth/resetPassword`: Resets the password with a token from the reset link.

---

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/password-reset-frontend.git
   cd password-reset-frontend
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

3. **Environment Variables**:
   - Create a `.env` file in the root directory with the following content:
     ```plaintext
     REACT_APP_API_URL=http://localhost:3000/api
     ```

4. **Run the Application**:
   ```bash
   npm start
   ```

5. **Test with Backend**:
   - Ensure the backend API server is running, and use a tool like Postman or test directly in the app.

---

## License

This project is licensed under the MIT License.