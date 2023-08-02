# FlexiAuth

[Try it out now](https://flex-auth-hi5a.vercel.app/login)

FlexiAuth is a web application providing a flexible authentication system, allowing users to sign up and log in using either email/password or Web3 authentication with their Ethereum wallets. It also supports Google OAuth for an even smoother login experience. JWT (JSON Web Tokens) is used for secure session management in both cases.

## 📑 Table of Contents

- [🚀 Features](#-features)
- [📝 User Flow](#-user-flow)
- [🛠️ Local Setup](#%EF%B8%8F-local-setup)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [🐳 Dockerization](#-dockerization)
- [🔧 Technologies Used](#-technologies-used)
- [🎉 Acknowledgement](#-acknowledgement)

## 🚀 Features

- **User Registration and Login:**
  - Implement user registration and login functionality with email/password authentication.
  - Users can sign up with an email and password and log in using their credentials.

- **Web3 Authentication Integration:**
  - Integrate Web3 authentication to allow users to log in using their Ethereum wallets (e.g., MetaMask, Trust Wallet).
  - Users can connect their Ethereum wallets securely to authenticate themselves.

- **Google OAuth Integration:**
  - Users can also log in using their Google accounts for a seamless login experience.

- **JWT-Based Session Management:**
  - Implement a JWT-based session management system for both email/password and Web3 authentication methods.
  - Users maintain their sessions securely using the JWT tokens.

- **Secure Storage of Credentials:**
  - Safely store user credentials and authentication-related information in the MongoDB database.
  - Use proper encryption and security measures to protect sensitive data.

- **Authentication Portability:**
  - Allow users to switch between email/password, Web3, and Google OAuth authentication methods seamlessly.

- **User Dashboard:**
  - Create a user dashboard that displays relevant information and allows users to manage their account settings.

- **Account Recovery Mechanism:**
  - Add an email-based account recovery mechanism for email/password authentication.


## 🔧 Technologies Used

- Front-end: **React.js**, **TypeScript**, **Figma** (for UI/UX design).
- Back-end: **Node.js**, **Express.js**, **TypeScript**.
- Database: **MongoDB**.
- Authentication: **JWT** for secure session management, **MetaMask** for Web3 authentication, and **Google OAuth** for smooth login experience.

## 📝 User Flow

1. Landing on the homepage
2. User Registration and Login options
3. Web3 Authentication process (if applicable)
4. Google OAuth process
5. Accessing and using the User Dashboard
6. Managing account settings and profile information
7. Account recovery mechanism (if applicable)
8. Other relevant user actions and interactions.

## 🛠️ Local Setup

To run this project locally, follow these steps:

### Prerequisites

- Node.js and npm installed on your system
- MongoDB running locally or accessible MongoDB URI

### Installation

1. Clone the repository:
```
git clone https://github.com/your-username/FlexiAuth.git
cd FlexiAuth
```

2. Install the dependencies on both client and server:
```
npm install
```

3. Set up environment variables:

Create a `.env` file in the root directory with the following environment variables:

```
PORT=3000
MONGODB_URI=your-mongodb-uri
JWT_SECRET=your-jwt-secret
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
```

Replace `your-mongodb-uri` with your MongoDB connection string, `your-jwt-secret` with a secure random string for JWT token generation, `your-google-client-id`, and `your-google-client-secret` with your Google OAuth client credentials.

### Running the Application

4. Run the development server on client folder:
```
npm run dev
```

5. The application should now be running at `http://localhost:3000`. Open your web browser and access this URL to use the application.

## 🐳 Dockerization

To run the project using Docker, make sure you have Docker installed on your system.

1. Build the Docker image:
```
docker build -t flexi-auth.
```

2. Run the Docker container:
```
docker run -p 3000:3000 -d flexi-auth.
```

3. The application should now be accessible at `http://localhost:3000`.
---
## 🎉 Acknowledgement
A sincere thank you to everyone who has directly or indirectly contributed to the success of this project. Your support and encouragement have been instrumental in making this endeavor possible. I am grateful for the opportunities, learnings, and memories gained during this project, and I look forward to future collaborations and improvements.


