# MERN Authentication App with Redux Toolkit and Firebase
Welcome ! This MERN (MongoDB, Express.js, React, Node.js) Authentication application is built with Redux Toolkit, Firebase, and Tailwind CSS. It includes Google OAuth for authentication.
## Live Demo

Visit the live website: [Live Demo](https://mern-auth-nlyn.onrender.com/)

## Table of Contents

- [Introduction](#introduction)
- [Use Case](#purpose)
- [Features](#features)
- [Technologies](#technologies)
- [Installation and Configuration](#installation)


## Introduction

This is a full-stack web application built with the MERN (MongoDB, Express, React, Node.js) stack. It includes authentication features that allow users to sign up, log in, and log out, and provides access to protected routes only for authenticated users.

The front-end of the application is built with React and uses React Router for client-side routing. The back-end is built with Node.js and Express, and uses MongoDB as the database. Authentication is implemented using JSON Web Tokens (JWT).

## Use Case
This application is intended as a starting point for building full-stack web applications with authentication using the MERN stack. Feel free to use it as a template for your own projects!

## Features

- User authentication using Firebase
- Google OAuth for easy login
- MERN Stack architecture
- State management with Redux Toolkit
- Responsive UI with Tailwind CSS

## Technologies

- MongoDB: Database for storing user information
- Express.js: Server-side framework for handling API requests
- React: Frontend library for building user interfaces
- Node.js: JavaScript runtime for server-side development
- Redux Toolkit: State management library for React applications
- Firebase: Authentication service and cloud storage
- Tailwind CSS: Utility-first CSS framework for styling

## Installation and Configuration

Clone the repository:

```bash
git clone https://github.com/your-username/your-mern-auth-app.git

# Navigate to the root folder of your project
cd your-mern-auth-app

# Install dependencies in the root folder
npm install

# Navigate to the client folder
cd client

# Install dependencies in the client folder
npm install

# Run the backend server in the root directory
npm run dev

# Run the development server in the client folder
npm run dev

## Firebase Configuration:

   - Create a Firebase project [here](https://console.firebase.google.com/).
   - Set up authentication in the Firebase console.
   - Obtain Firebase configuration details.

     Example Firebase configuration (`src/firebase.js`):

     ```javascript
     // src/firebase.js

     import { initializeApp } from 'firebase/app';
     import { getAuth } from 'firebase/auth';

     const firebaseConfig = {
       apiKey: 'your-firebase-api-key',
       authDomain: 'your-firebase-auth-domain',
       projectId: 'your-firebase-project-id',
       storageBucket: 'your-firebase-storage-bucket',
       messagingSenderId: 'your-firebase-messaging-sender-id',
       appId: 'your-firebase-app-id',
     };

     const app = initializeApp(firebaseConfig);
     const auth = getAuth(app);

     export { auth };
     ```

## Environment Variables:

   - Create a `.env` file in the root directory of your project.
   - Add necessary environment variables for your application.

     Example `.env` file:

     ```env
     # MongoDB Connection String
     MONGODB_URI=your-mongodb-connection-string

     # Firebase Configuration
     REACT_APP_FIREBASE_API_KEY=your-firebase-api-key
     REACT_APP_FIREBASE_AUTH_DOMAIN=your-firebase-auth-domain
     REACT_APP_FIREBASE_PROJECT_ID=your-firebase-project-id
     REACT_APP_FIREBASE_STORAGE_BUCKET=your-firebase-storage-bucket
     REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your-firebase-messaging-sender-id
     REACT_APP_FIREBASE_APP_ID=your-firebase-app-id
     ```

   - Update the values in the `.env` file with your actual configuration details.

Make sure to replace placeholder values like `your-firebase-api-key`, `your-mongodb-connection-string`, etc., with your actual configuration details.
