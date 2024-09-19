# College Directory Application

A web application designed to facilitate seamless interaction between students, faculty members, and administrators within a college. The platform allows users to manage and access personal and academic information efficiently.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

---

## Features

### 1. Login Functionality
- Secure login system with role-based authentication (Student, Faculty Member, Administrator).
- Redirects users to their respective dashboards based on role.

### 2. Student Dashboard
- View personal profile information (photo, contact details, courses, grades, and attendance).
- Search for other students by name, department, or year.
- Contact faculty advisors via email or phone.

### 3. Faculty Dashboard
- Manage class lists: view students with their names, photos, and contact information.
- Update personal profile with office hours, contact email, and phone number.

### 4. Administrator Dashboard
- Manage student and faculty records: add, update, or remove records.
- View data visualization charts for key metrics like student enrollment trends and faculty course loads.

## Technologies

### Frontend:
- **React**: UI library for building responsive user interfaces.
- **CSS**: For styling the application.
- **React Router**: For routing and navigation.
- **Axios**: For making HTTP requests to the backend.

### Backend:
- **Node.js**: JavaScript runtime for building server-side logic.
- **Express.js**: Web framework for creating RESTful APIs.
- **JWT**: For authentication and session management.
- **MongoDB**: NoSQL database for storing application data.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/college-directory.git
   cd college-directory
2. Install the dependencies for the frontend:

  ```bash
    cd frontend
    npm install
  ```
3. Install the dependencies for the backend:
   ```bash
   cd backend
   npm install
   ```
4. Start the frontend development server:
  ```bash
    cd frontend
    npm start
  ```
5. Start the backend server:
   ```bash
   cd backend
   npm run dev
   ```

## Usage

1. Go to `http://localhost:3000/login` in your browser.
2. Log in with one of the three roles: **Student**, **Faculty Member**, or **Administrator**.
3. Depending on the role, you will be redirected to the appropriate dashboard.

### Example Logins:

- **Student**: Use the credentials created during user registration or provided during the installation setup.
- **Faculty**: Faculty credentials can be added via the admin panel or provided during setup.
- **Admin**: Admin credentials can be added manually or through the setup process.


## Folder Structure

```
college-directory/
│
├── backend/                    # Node.js Express Backend
│   ├── src/                    # Source code for backend
│   ├── models/                 # Database models
│   ├── controllers/            # Business logic
│   ├── routes/                 # API routes
│   ├── config/                 # Configuration files (e.g., for database and JWT)
│   └── server.js               # Entry point for the backend
│
├── frontend/                   # React Frontend
│   ├── src/
│   │   ├── components/         # Reusable components (Login, Dashboard, etc.)
│   │   ├── pages/              # Role-specific pages (Student, Faculty, Admin)
│   │   └── redux/              # Redux state management
│   ├── App.js                  # Main application component
│   ├── index.js                # Application entry point
│   ├── Login.css               # Styling for login page
│   └── ...

```

## API Endpoints

- **POST** `/api/auth/login`: Authenticate user and provide JWT token.
- **GET** `/api/student/profile`: Fetch student profile information.
- **GET** `/api/faculty/classes`: Fetch class list for faculty members.
- **POST** `/api/admin/student`: Add or update student record.
- **GET** `/api/admin/dashboard`: Get aggregated data for visualizations.







   


