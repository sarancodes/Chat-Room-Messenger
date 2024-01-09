# Chat Room Messenger

A room chat messenger built using React JS and firebase.

## Components

#### 1.Frontend
This is the user interface that users interact with. It is built using React and consists of several components, including:

> Authentication component: This component handles user login and authentication using Firebase Authentication.

> Room selection component: This component allows users to enter a room name and join a chat room.

> Chat component: This component displays the chat messages and allows users to send new messages

#### 2.Firebase
This is the backend that provides the data storage and authentication for the application. It consists of two main components:

> Firebase Authentication: This service handles user login and authentication.

> Firestore: This is a NoSQL database that stores the chat messages for each room.

#### 3.Cookies 
The application uses cookies to store the user's authentication token. This allows the user to stay logged in even if they refresh the page.


## Process Flow
- When a user opens the application, the frontend component checks if the user is already logged in.
- If not, the user is prompted to sign in using Firebase Authentication.
- Once the user is logged in, the frontend component displays the room selection component.
- The user enters a room name and clicks the "Enter Chat" button.
- The frontend component sends a request to Firestore to get the chat messages for the specified room.
- Firestore returns the chat messages to the frontend component.
- The frontend component displays the chat messages in the chat component.
- When the user types a new message, the frontend component sends the message to Firestore.
- Firestore stores the message in the database.
- The frontend component updates the chat component to display the new message.

## Architecture 
![Architecture](https://github.com/sarancodes/Chat-Room-Messenger/blob/main/Architecture.png)

## Deploy your own 
- Clone the repository
- Change directory to inside the folder
- Add an .env file with your firebase configs
- Run npm install
- Start the server
- View it on localhost:3000
```sh
cd Chat-Room-Messenger
npm install
npm start
```


