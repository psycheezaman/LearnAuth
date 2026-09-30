# LearnAuth
"LearnAuth" is a full-stack user authentication and management application developed using Flutter and Django REST Framework. The main objective of the project is to provide a simple, secure, and user-friendly system for account registration, email verification, login, and user access management. The Flutter framework is used to build the mobile application interface, while Django REST Framework provides the backend APIs and manages user authentication and database operations. "LearnAuth" demonstrates the practical implementation of mobile application development, RESTful API integration, user authentication, and email verification in a client-server architecture. The project also serves as a foundation for future applications that require secure user registration and authentication features.

## Technology Stack

LearnAuth is developed using a modern client-server architecture where the mobile application communicates with a backend server through REST APIs.

### Frontend
The frontend of LearnAuth is developed using Flutter and Dart. Flutter is used to create the mobile user interface, while Dart is used to implement the application logic. The frontend handles user registration, login, OTP verification, dashboard navigation, and communication with the backend.

### Backend
The backend is developed using Django and Django REST Framework. Django manages the application logic, user model, authentication process, and database operations. Django REST Framework is used to create RESTful API endpoints that allow the Flutter application to exchange data with the server.

### Database
**SQLite** is used as the database during development. It stores user information such as email addresses, encrypted passwords, verification status, and OTP-related data.

### API Communication
The Flutter application communicates with the backend through HTTP requests. REST API endpoints are used for registration, login, and OTP verification.

### Authentication and Security
Django's built-in password hashing mechanism is used to protect user passwords. The system also includes **email-based OTP verification** to confirm user identity before allowing full access to the application.

### Development Tools
The project has developed by using Android Studio.

---

## Key Features

### User Registration
Users can create a new account using their email address and password. The submitted information is sent to the Django backend through a REST API.

### Email OTP Verification
After registration, the system generates an OTP and uses it to verify the user's email address. This helps ensure that the registered email belongs to the actual user.

### Secure Login
Verified users can log in using their registered email address and password. The backend validates the submitted credentials before granting access.

### Custom User Authentication
LearnAuth uses a custom user model where the email address is used as the primary identity for authentication instead of a traditional username.

### Dashboard Access
After successful authentication, users are redirected to a dashboard that confirms successful login and provides access to authenticated areas of the application.

### Password Security
User passwords are not stored as plain text. Django's built-in password hashing system is used to store them securely in the database.

### REST API Integration
The frontend and backend are separated and communicate using RESTful APIs. This architecture makes the system easier to maintain and extend.

### Cross-Platform Development
Because the frontend is developed using Flutter, the application can be adapted for multiple platforms such as Android and iOS with a largely shared codebase.

### User-Friendly Interface
The application provides a simple and straightforward interface for registration, verification, login, and dashboard navigation.

### Expandable Architecture
LearnAuth can be extended in the future with additional features such as password recovery, user profiles, JWT authentication, role-based access control, and integration with a production database such as PostgreSQL.

