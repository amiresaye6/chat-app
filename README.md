# MERN Stack Chat Application

## Overview
This project is a real-time chat application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) with WebSocket integration via Socket.io. It features user authentication, real-time messaging, chat rooms, and persistent message storage.

## Features
- **User Authentication**: Secure registration, login, and logout using JWT.
- **Real-Time Messaging**: Instant messaging with Socket.io for real-time communication.
- **Chat Rooms**: Support for multiple chat rooms and private messaging.
- **Persistent Storage**: Messages are stored in MongoDB, allowing users to view chat history.
- **Responsive UI**: User-friendly and responsive interface built with React and Tailwind CSS.

## Tech Stack
- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Real-Time Communication**: Socket.io
- **Authentication**: JWT (JSON Web Token)

## Getting Started

### Prerequisites
- **Node.js**: Install from [nodejs.org](https://nodejs.org/)
- **MongoDB**: Install and run MongoDB locally or use a cloud service like MongoDB Atlas.

### Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/chat-app.git
    cd chat-app
    ```

2. **Install Dependencies**:
    - Backend:
      ```bash
      cd server
      npm install
      ```
    - Frontend:
      ```bash
      cd ../client
      npm install
      ```

3. **Environment Variables**:
    - Create a `.env` file in the `server` directory with the following content:
      ```env
      MONGO_URI=your_mongodb_connection_string
      JWT_SECRET=your_jwt_secret
      PORT=5000
      ```
    - Create a `.env` file in the `client` directory if necessary for any frontend environment variables.

### Running the Application

1. **Start the Backend**:
    ```bash
    cd server
    npm start
    ```

2. **Start the Frontend**:
    ```bash
    cd ../client
    npm start
    ```

3. **Access the Application**:
    - Open your browser and navigate to `http://localhost:3000`.

## Project Structure

- **/server**: Contains the backend code.
  - **/models**: Mongoose models for Users and Messages.
  - **/routes**: API routes for authentication and chat features.
  - **/controllers**: Logic for handling API requests.
  - **/socket**: Socket.io configuration and event handling.
- **/client**: Contains the frontend code.
  - **/src/components**: React components for the UI.
  - **/src/context**: Context API for global state management.
  - **/src/pages**: Main pages like Login, Register, and Chat.

## Key Features

### User Authentication
- Secure user registration and login using JWT.
- Passwords are hashed using bcrypt.

### Real-Time Messaging
- Implemented using Socket.io for real-time communication.
- Users can join chat rooms or have private conversations.

### Persistent Storage
- Messages are stored in MongoDB, allowing users to retrieve chat history.

## Deployment

1. **Backend Deployment**: Use platforms like Heroku, AWS, or DigitalOcean.
2. **Frontend Deployment**: Use platforms like Netlify, Vercel, or Heroku.
3. **WebSocket Deployment**: Ensure that Socket.io works properly in your production environment.

## Additional Features
- **Push Notifications**: Implement push notifications for new messages.
- **Media Sharing**: Allow users to share images, videos, and files.
- **Typing Indicators**: Show when a user is typing in a chat.
- **Read Receipts**: Indicate when a message has been read.

## Security Considerations
- Secure WebSocket connections using SSL/TLS.
- Validate all user inputs to prevent security vulnerabilities like SQL injection and XSS.
- Ensure user passwords are hashed using bcrypt.

## Contributing
Feel free to submit issues and pull requests to contribute to the project.

## License
This project is licensed under the MIT License.

## Acknowledgements
- Thanks to the creators of the MERN stack, Socket.io, and Tailwind CSS for their amazing tools.
