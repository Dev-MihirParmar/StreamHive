
# StreamHive

StreamHive is a platform where users can upload, view, and share video tutorials on a wide range of topics. The platform includes user authentication, secure video uploads, and a responsive frontend to interact with the video content.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Running the Project](#running-the-project)
- [API Endpoints](#api-endpoints)
- [Frontend Routes](#frontend-routes)
- [License](#license)

## Features
- User Authentication (Registration and Login)
- Secure Video Uploads
- Video Streaming
- Responsive UI

## Tech Stack
- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Frontend:** React.js, React Router, Axios, Video.js
- **Authentication:** JSON Web Tokens (JWT)
- **File Uploads:** Multer

## Prerequisites
Before you begin, ensure you have met the following requirements:
- Node.js and npm installed
- MongoDB installed and running

## Installation

### Backend Setup
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd streamhive-backend
    ```

2. Install the dependencies:
    ```bash
    npm install
    ```

3. Create a `.env` file in the root directory of the backend project with the following content:
    ```ini
    PORT=5000
    MONGO_URI=mongodb://localhost:27017/streamhive
    JWT_SECRET=your_jwt_secret
    ```

### Frontend Setup
1. Navigate to the frontend directory:
    ```bash
    cd streamhive-frontend
    ```

2. Install the dependencies:
    ```bash
    npm install
    ```

## Environment Variables
Create a `.env` file in the root directory of the backend project with the following content:
```ini
PORT=5000
MONGO_URI=mongodb://localhost:27017/streamhive
JWT_SECRET=your_jwt_secret
```

## Running the Project

### Backend
To start the backend server, run the following command in the `streamhive-backend` directory:
```bash
npm start
```

### Frontend
To start the frontend development server, run the following command in the `streamhive-frontend` directory:
```bash
npm start
```

## API Endpoints
- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - Login a user
- **POST** `/api/video/upload` - Upload a video (requires authentication)
- **GET** `/api/video/:id` - Get video by ID

## Frontend Routes
- `/login` - User login page
- `/register` - User registration page
- `/upload` - Video upload page (requires authentication)
- `/video/:id` - Video player page

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
