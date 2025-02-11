# Backend Project

This repository contains the backend for a video streaming platform similar to YouTube. It handles user authentication, media uploads, interactions (likes, comments, subscriptions), playlist management, system health checks, dashboard analytics, and tweet functionalities.

## Technologies Used

- **Node.js**: A JavaScript runtime for server-side execution.
- **Express.js**: A lightweight and flexible framework for building APIs and handling HTTP requests.
- **MongoDB**: A NoSQL database used for storing structured and unstructured data.
- **Mongoose**: An ODM library that simplifies MongoDB interactions by providing schema-based data modeling.
- **Cloudinary**: A cloud-based service for managing and optimizing images and videos.
- **Multer**: A middleware for processing multipart/form-data, primarily for handling file uploads.
- **JWT (JSON Web Token)**: A mechanism for secure user authentication and authorization.
- **Prettier**: A formatting tool to enforce a consistent coding style across the project.
- **Cookie-parser**: A middleware for parsing and managing cookies in HTTP requests.
- **CORS**: Middleware to enable Cross-Origin Resource Sharing, allowing API access from different domains.
- **Dotenv**: A module for managing environment variables, keeping sensitive configurations secure.
- **Bcrypt**: A library used to hash passwords, ensuring secure authentication.

## Features

### Controllers

- **User Controller**: Handles user-related functionalities, including account creation, login, logout, profile updates, and password changes.
- **Video Controller**: Manages video uploads, updates, and retrieval.
- **Comment Controller**: Controls commenting features on videos.
- **Tweet Controller**: A new addition that enables users to post and interact with tweets.
- **Like Controller**: Handles likes for both videos and tweets.
- **Playlist Controller**: Manages user-created playlists.
- **Subscription Controller**: Oversees user subscription features.
- **Healthcheck Controller**: Provides API endpoints for monitoring server health.
- **Dashboard Controller**: Manages data insights for the platform’s analytics dashboard.

### Middleware

Middleware functions play a crucial role in handling request processing, authentication, logging, and error management. They allow pre-processing or validation before passing data to controllers.

### Cloudinary Integration

Cloudinary is used in this project for media asset management, enabling efficient storage, processing, and retrieval of images and videos, such as profile pictures, thumbnails, and cover images.

### Multer for File Handling

Multer simplifies handling multipart/form-data, allowing seamless uploading of media files like avatars, cover images, and videos.

### JSON Web Tokens (JWT)

JWT is employed to authenticate users securely. It generates access and refresh tokens that manage session persistence and authorization within the platform.

### Prettier for Code Formatting

Prettier ensures a standardized coding style, making the project’s codebase more readable and maintainable.

### Cookie-parser Middleware

This middleware is used to parse cookies in incoming HTTP requests, making cookie management straightforward in Express applications.

### CORS Configuration

CORS (Cross-Origin Resource Sharing) middleware enables API access from different domains while maintaining security protocols.

### Dotenv for Environment Variables

Dotenv loads environment-specific variables from a `.env` file into `process.env`, helping to keep sensitive information like API keys and database credentials secure.

### Bcrypt for Password Security

Bcrypt hashes user passwords before storing them in the database, preventing unauthorized access through brute-force attacks or credential leaks.
