# TASK 2 – Real-Time Chat Application using WebSockets

*COMPANY*: CODTECH IT SOLUTIONS  
*NAME*: MAADESHWAR D V  
*INTERN ID*: CITS0D500  
*DOMAIN*: FULL STACK DEVELOPMENT  
*DURATION*: 4 WEEKS  
*MENTOR*: NEELA SANTOSH  

## Description:

For Task 2 of my full-stack internship, I was tasked with building a **Real-Time Chat Application** using **WebSockets**, with **Socket.io** as the core library for enabling real-time bidirectional communication. The objective was to simulate a basic version of modern chat applications like WhatsApp, Messenger, or Discord, where users can communicate instantly and see live updates without page refreshes.

To achieve this, I used **Node.js** and **Express.js** for the backend server, and **HTML, CSS, and JavaScript** for the frontend interface. **Socket.io**, a real-time engine built on WebSockets and HTTP fallback protocols, was used both on the server and client sides to manage real-time events such as sending and receiving messages, user join/leave notifications, and more.

The first step was to set up the backend server with Express. I created a basic HTTP server and integrated Socket.io on top of it. The server listens for client connections and manages events like `connection`, `disconnect`, and custom events such as `chatMessage` and `userJoined`. When a user sends a message, the server broadcasts it to all connected users in the room. Similarly, when a new user joins or leaves, the server informs others in real time.

On the frontend, I built a simple yet responsive chat interface. Users are prompted to enter a username when joining the chat room. After entering, they can type and send messages which are displayed in the message box with timestamps and username tags. I added features like auto-scroll to the newest message, a visual typing indicator (optional), and event-driven DOM updates based on socket messages.

A key learning point in this task was **event-driven programming**. Both the client and server communicate using custom event names. For example, when a message is typed and submitted, a `sendMessage` event is emitted, which the server listens to and then emits a `receiveMessage` event to all clients. This architecture helps keep both ends of the application loosely coupled yet tightly synchronized in behavior.

I also implemented basic user management logic. Each new connection is stored in an array or map on the server side, allowing us to keep track of online users. When a user disconnects, a `userLeft` event is broadcast, and the user is removed from the list. Though this version was kept simple, it gave me exposure to session management and scalability considerations for multi-user apps.

For styling, I used CSS Grid and Flexbox to design a clean, responsive chat interface. Messages are aligned left or right depending on the sender, and new messages animate in smoothly. I also ensured keyboard accessibility and responsive layout behavior across different devices.

This task was a turning point in my understanding of how **real-time applications** work under the hood. It showed me how chat apps, collaborative tools, and multiplayer games manage instant data updates. More importantly, it introduced me to **WebSockets**, which allow full-duplex communication between client and server, unlike traditional request-response HTTP systems.

Finally, this task emphasized the need for performance optimization, error handling, and secure connection management, which are crucial when building scalable real-time systems. With further improvements like adding rooms, private messaging, or user authentication, this project can evolve into a production-level messaging app.

In conclusion, Task 2 gave me a solid foundation in real-time full-stack development. I learned how to build an event-driven architecture using Socket.io, integrate it with Node.js and Express, and create dynamic frontend experiences. The hands-on experience from this task has prepared me for more complex real-time collaborative applications in the future.

## Output 
Click to view the website
🔗 [https://madex-tech.github.io/chat-frontend/](https://madex-tech.github.io/chat-frontend/)

<img width="1919" height="870" alt="Screenshot 2025-07-13 113125" src="https://github.com/user-attachments/assets/457d455d-abb4-4796-8558-21991f08ffaf" />

