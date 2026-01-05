💬 Real-Time Chat Application
A full-stack, responsive chat platform that enables users to communicate instantly through text and media. Built with Socket.io for low-latency, bi-directional communication.

https://quick-gpt-ydkw.onrender.com

🚀 Features
Real-Time Messaging: Instant text delivery using WebSockets.

Media Sharing: Send and receive photos seamlessly.

Live Connection Status: Real-time "User Online/Offline" indicators.

Responsive UI: Optimized for both desktop and mobile using Tailwind CSS v4.

Dynamic Rooms: Support for multiple chat rooms or private 1-on-1 messaging.

Optimistic UI Updates: Messages appear instantly on the sender's screen for a smooth user experience.

🛠️ Tech Stack
Frontend
React + Vite: For a fast, modern UI development experience.

Socket.io-client: To manage the persistent connection to the server.

Tailwind CSS v4: For high-performance, utility-first styling.

Backend
Node.js & Express: The foundation of the server-side logic.

Socket.io: To handle the real-time event-based communication.

Base64: (Mention whichever you used) for handling image uploads and processing.

🏗️ How It Works
The application utilizes a Client-Server-Client architecture.

Connection: When a user opens the app, a handshake is performed between the Vite frontend and the Node.js backend to establish a persistent WebSocket connection.

Event Emission: When a user sends a message or photo, the client "emits" an event to the server.

Broadcasting: The server receives the data and "broadcasts" it to the specific room or recipient.

Binary Handling: Photos are processed as binary data or base64 strings, ensuring they are delivered without needing a traditional page refresh.

⚙️ Installation & Setup

Clone the repository:

Bash

git clone https://github.com/gauravdevkar27/chat_app.git
Install dependencies for both Client and Server:

Bash

# In the root or server folder
cd server && npm install

# In the client folder
cd client && npm install

Environment Variables: Create a .env file in the server directory:

Code snippet

PORT=5000
CLIENT_URL=http://localhost:5173

Run the Application:

Bash

# Start server
npm run server

# Start client (in a separate terminal)
cd client && npm run dev

Socket.io: To handle the real-time event-based communication.

Multer / Base64: (Mention whichever you used) for handling image uploads and processing.
