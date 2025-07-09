
# FullStack Web Application

## Project Overview

This project is a FullStack Web Application . It leverages Node.js with Express and MongoDB for the backend, and Angular with Angular Material for the frontend. The application supports functionalities such as CRUD operations for managing accounts, questions, and candidates, role-based access control, and a responsive user interface.

---

## Table of Contents

1. [Project Structure](#project-structure)
2. [Technologies Used](#technologies-used)
3. [Installation and Setup](#installation-and-setup)
4. [Running the Application](#running-the-application)
5. [Features](#features)
6. [API Documentation](#api-documentation)
7. [Usage Instructions](#usage-instructions)
8. [Contributing](#contributing)
9. [License](#license)

---

## Project Structure

The project is structured into two main parts: the backend and the frontend.

### Backend
- **Technologies:** Node.js, Express, MongoDB, Mongoose, TypeScript
- **Directory Structure:**
  - `src/`
    - `controllers/` - Contains the controllers that handle the requests and responses.
    - `models/` - Contains the Mongoose models defining the data structure.
    - `routes/` - Defines the API routes and their handlers.
    - `services/` - Contains services that handle business logic, like authentication and data manipulation.
    - `middlewares/` - Contains middleware for handling authentication, error handling, etc.
    - `config/` - Configuration files, including database setup.

### Frontend
- **Technologies:** Angular, Angular Material, RxJS
- **Directory Structure:**
  - `src/`
    - `app/`
      - `components/` - Contains all Angular components (e.g., question-list, question-edit, login).
      - `services/` - Angular services to interact with the backend.
      - `models/` - TypeScript interfaces and models for the application’s data.
      - `modules/` - Angular modules for organizing components and services.
    - `assets/` - Contains static assets like images, icons, etc.
    - `styles/` - Global styles for the application.

---

## Technologies Used

### Backend
- **Node.js:** Server-side runtime for JavaScript.
- **Express:** Web framework for building RESTful APIs.
- **MongoDB:** NoSQL database for storing data.
- **Mongoose:** ODM for MongoDB to manage data.
- **TypeScript:** Superset of JavaScript providing static typing.

### Frontend
- **Angular:** Frontend framework for building SPAs.
- **Angular Material:** UI component library based on Material Design.
- **RxJS:** Library for reactive programming with observables.

---

## Installation and Setup

### Prerequisites

- Node.js and npm installed on your machine.
- MongoDB setup and running locally or on Atlas.

### Backend Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/assessment-app.git
   cd assessment-app
   ```

2. **Install Backend Dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Environment Configuration:**
   - Create a `.env` file in the `backend` directory and configure the following:
     ```plaintext
     MONGO_URI=<your_mongodb_connection_string>
     JWT_SECRET=<your_jwt_secret_key>
     PORT=5000
     ```

4. **Run the Backend Server:**
   ```bash
   npm run start
   ```

### Frontend Setup

1. **Navigate to Frontend Directory:**
   ```bash
   cd ../frontend
   ```

2. **Install Frontend Dependencies:**
   ```bash
   npm install
   ```

3. **Run the Frontend Server:**
   ```bash
   ng serve
   ```

---

## Running the Application

To run the application locally:

1. Ensure that your MongoDB instance is running.
2. Start the backend server using `npm run start` in the `backend` directory.
3. Start the frontend Angular application using `ng serve` in the `frontend` directory.
4. Open your browser and navigate to `http://localhost:4200`.

---

## Features

### Backend
- **CRUD Operations:** Create, Read, Update, Delete operations for managing accounts, questions, and candidates.
- **Role-Based Access Control:** Different roles (Admin, Delivery Admin) with specific access rights.
- **Authentication:** Secure login with JWT-based authentication.

### Frontend
- **Single-Page Application:** Built using Angular for seamless navigation and interaction.
- **Responsive Design:** UI components are responsive, ensuring usability across devices.
- **Question Management:** Interface for listing, editing, and deleting questions.
- **Candidate Management:** Interface for listing, filtering, and managing candidates.
- **Login System:** Secure login form with session persistence.

---

## API Documentation

### Example Endpoints

- **POST /api/login:** Authenticates a user and returns a JWT token.
- **GET /api/questions:** Retrieves a list of all questions.
- **POST /api/questions:** Adds a new question.
- **PUT /api/questions/:id:** Updates an existing question.
- **DELETE /api/questions/:id:** Soft deletes a question.
- **GET /api/candidates:** Retrieves a list of all candidates.

---

## Usage Instructions

### Admin User
- **Login:** Use the login page to authenticate as an admin.
- **Manage Questions:** Navigate to the questions module to add, edit, or delete questions.
- **Manage Candidates:** Access the candidates module to view, filter, or manage candidate data.

### Delivery Admin User
- **Login:** Authenticate using your credentials.
- **Access Candidates:** Navigate to the candidates module to manage candidate information.

---

## Contributing

1. **Fork the Repository**
2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/YourFeature
   ```
3. **Commit Your Changes**
   ```bash
   git commit -m "Add your message here"
   ```
4. **Push to the Branch**
   ```bash
   git push origin feature/YourFeature
   ```
5. **Create a Pull Request**

---

## License

This project is licensed  - see the LICENSE.md file for details.

---

This README file provides a comprehensive guide to understanding, setting up, and contributing to the project. It covers the project structure, technologies used, installation instructions, and how to run and use the application.
