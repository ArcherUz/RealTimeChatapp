# Chat Application

This real-time chat application is built using Node.js, Express, and Socket.io. Users can join different chat rooms or create their own rooms. They can send and receive messages in real time and even share their location.

## Features

- **Real-time Messaging**: With Socket.io, users can send and receive messages in real time.
- **Profanity Check**: Messages are checked for profanity using the `bad-words` library. Users are notified if they use inappropriate words.
- **Dynamic Room Support**: Users can join existing rooms or even create new ones.
- **User List**: Each room displays a list of users currently present.
- **Location Sharing**: Users have the ability to share their location, which is sent as a Google Maps link to the chat room.
- **User Status**: The app notifies the room when a user joins or leaves.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Node.js
- NPM (Node Package Manager)

### Setup & Installation

1. **Clone the Repository**
    ```bash
    git clone [Repository URL]
    ```

2. **Navigate to Project Directory**
    ```bash
    cd [Project Directory]
    ```

3. **Install Dependencies**
    ```bash
    npm install
    ```

4. **Run the App**

    For development:
    ```bash
    npm run dev
    ```

    For production:
    ```bash
    npm start
    ```

5. **Access the App**: Open a browser and visit `http://localhost:3000`.

## Usage

1. **Joining a Room**: Provide a username and room name.
2. **Sending Messages**: Use the message box. Hit Enter or click "Send".
3. **Share Location**: Use the "Share Location" button.
4. **Active Users**: View users in the current room via the sidebar.

## Code Structure

- **index.js**: This is the main server file. It handles socket connections, room joins, message sending, and location sharing.
- **chat.js**: Client-side functionality. Handles sending messages, sharing location, and UI updates.
- **user.js**: Utility functions for user management like adding, removing, and fetching users from rooms.

## Dependencies

- **bad-words**: This library is utilized to filter out profanity in messages.
- **env-cmd**: A tool to run commands with an environment sourced from a file.
- **express**: A fast, minimalist web framework for Node.js.
- **socket.io**: Enables real-time bidirectional event-based communication.

