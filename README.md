# LevChat - Real-time Chat Room

LevChat is a real-time chat room web application built using Python, Flask and Socket.IO. It allows users to create and join chat rooms where they can exchange messages in real-time.

![LevChat Screenshot](screenshots/2.png)
![LevChat Screenshot](screenshots/1.png)


## Features

- Create a new chat room with a unique random code.
- Join an existing chat room using a room code from your friend.
- Real-time messaging with other users in the same chat room.
- Displays the names of users who are currently in the room.
- Automatic room deletion when all users leave the room.

## Technologies Used

- [Flask](https://flask.palletsprojects.com/en/2.1.x/): A Python web framework used for serving web pages and handling HTTP requests.
- [Socket.IO](https://socket.io/): A library for real-time, bidirectional communication between the server and clients.
- HTML/CSS: Used for designing and structuring the web pages.
- JavaScript: Used for handling client-side functionality and communication with the server.

## How It Works

1. **Home Page**:
   - Users can enter their name and choose to either join an existing chat room by entering a room code or create a new chat room.
   - Validation checks ensure that users provide a name and, if joining a room, a valid room code.

2. **Chat Room**:
   - Users are redirected to a chat room upon successful entry.
   - Real-time messages are displayed in the chat area.
   - Users can send messages by typing in the message input field and clicking the "Send" button.
   - When a user enters or leaves the room, a notification is displayed in the chat.

3. **Server-Side**:
   - Flask handles routing, rendering HTML templates, and processing form submissions.
   - Socket.IO is used to establish WebSocket connections for real-time messaging.
   - Messages are broadcasted to all users in the same chat room using Socket.IO events.

## Setup and Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/levchat.git

2. Install the required Python packages:
 
    ```bash
    pip install -r requirements.txt

3. Run the Flask application:

    ```bash
    python main.py

4. Open your web browser and access the application at http://localhost:5000.