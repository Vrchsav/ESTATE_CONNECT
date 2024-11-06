# 🏡 MERN Estate Platform

Welcome to the MERN Estate Platform! This project is a modern, feature-rich real estate application that leverages the power of the MERN (MongoDB, Express, React, Node.js) stack. It allows users to explore property listings, contact agents, and manage their real estate needs effortlessly. 

![Real Estate Platform](./client/src/assets/Screenshot%202024-11-06%20081402.png)

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Environment Variables](#environment-variables)
- [Usage Guide](#usage-guide)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)



## About the Project

The MERN Estate Platform is a full-featured application designed to connect property buyers, sellers, and agents. Users can browse listings, view detailed property information, save favorites, and contact agents directly through the app. Agents can manage listings and receive inquiries in real time.

## Features

- **User Authentication**: Sign up, log in, and manage user sessions securely using JWT.
- **Property Listings**: Browse, filter, and view detailed information on properties.
![Property Listings](./client/src/assets/Screenshot%202024-11-06%20081424.png)
- **Favorites**: Save favorite listings for easy access.
![Favorites](./client/src/assets/Screenshot%202024-11-06%20081504.png)
- **Agent Profiles**: Connect with agents and view their listings.
- **Responsive Design**: Fully optimized for desktops, tablets, and mobile devices.
![Responsive Design](./client/src/assets/Screenshot%202024-11-06%20082222.png)
- **Admin Dashboard**: An interface for managing property listings and user roles.
![Admin Dashboard](./client/src/assets/Screenshot%202024-11-06%20081556.png)
- **Real-time Notifications**: Get notified of new listings and inquiries.

## Tech Stack

| Layer          | Technology                   |
|----------------|------------------------------|
| **Frontend**   | React, CSS, Bootstrap        |
| **Backend**    | Node.js, Express             |
| **Database**   | MongoDB                      |
| **Authentication** | JWT (JSON Web Tokens)    |
| **Hosting**    | Deployed on **AWS** or **Heroku**  |



## Project Structure

The project is structured to separate concerns across different directories:

```plaintext
mern-estate-main/
├── client/                  # Frontend code (React)
│   ├── src/
│   ├── public/
│   ├── package.json         # Frontend dependencies
│   └── ...
├── server/                  # Backend code (Express)
│   ├── controllers/         # Logic for handling requests
│   ├── models/              # Mongoose models
│   ├── routes/              # API route definitions
│   ├── config/              # Configuration files
│   ├── middleware/          # Authentication and validation
│   ├── server.js            # Entry point for backend
│   └── ...
└── README.md                # Project documentation
```





## Setup and Installation 

### Prerequisites 
 
- [Node.js](https://nodejs.org/)  (v14+ recommended)
 
- [MongoDB](https://www.mongodb.com/)  (local or cloud instance)
 
- [Git](https://git-scm.com/)

### Installation 
 
 1. **Clone the repository:** 

    ```bash
    git clone https://github.com/yourusername/mern-estate.git
    cd mern-estate-main
    ```
 
2. **Install dependencies for both frontend and backend:** 
    #### Frontend Installation 


    ```bash
    cd client
    npm install
    ```

    #### Backend Installation 


    ```bash
    cd ../server
    npm install
    ```

### Environment Variables 
Create a `.env` file in the `server` directory and add the following environment variables:

```plaintext
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```





## Usage Guide 
 
1. **Start the Backend Server:** 

    ```bash
    cd server
    npm run dev
    ```
 
2. **Start the Frontend Server:** 

    ```bash
    cd ../client
    npm start
    ```
 
3. **Access the Application:**  
  - **Frontend** : `http://localhost:3000`
 
  - **Backend API** : `http://localhost:5000`





## API Endpoints 

### Authentication 
 
- `POST /api/auth/register` - Register a new user.
 
- `POST /api/auth/login` - Log in a user.

### Properties 
 
- `GET /api/properties` - Retrieve all properties.
 
- `GET /api/properties/:id` - Get specific property details.
 
- `POST /api/properties` - Create a new property (Admin only).
 
- `PUT /api/properties/:id` - Update a property (Admin only).
 
- `DELETE /api/properties/:id` - Delete a property (Admin only).

### Users 
 
- `GET /api/users` - Get user information (Admin only).
 
- `PUT /api/users/:id` - Update user information (Admin only).





## Contributing 

We welcome contributions to make this project even better. To contribute:

1. Fork the project.
 
2. Create a new branch for your feature or fix (`git checkout -b feature/AmazingFeature`).
 
3. Commit your changes with clear, concise messages (`git commit -m 'Add some AmazingFeature'`).
 
4. Push to the branch (`git push origin feature/AmazingFeature`).

5. Open a pull request describing your changes.
