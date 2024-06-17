## Description

ChatZo is an advanced chat application designed for secure and efficient instant communication. It leverages JWT Authentication and WebSocket technology to provide seamless real-time messaging capabilities. Built with modern technologies, ChatZo ensures a smooth user experience with robust security features.

## Key Features

- **JWT Authentication:** Secure user authentication using JSON Web Tokens (JWT), ensuring data integrity and user privacy.
- **WebSocket Technology:** Enables real-time communication, allowing users to send and receive messages instantly.
- **Next.js & TypeScript:** Frontend developed with Next.js for server-side rendering and TypeScript for enhanced code reliability and maintainability.
- **Tailwind CSS:** Utilizes Tailwind CSS for a responsive and customizable user interface, ensuring a sleek design and smooth user experience.
- **Golang Backend:** Backend implemented in Golang (Go), known for its efficiency and concurrency support, ensuring high performance and scalability.

## Technologies Used

- **Frontend:** Next.js, TypeScript, Tailwind CSS
- **Backend:** Golang (Go)
- **Authentication:** JWT
- **Real-Time Communication:** WebSocket

ChatZo is ideal for applications requiring real-time messaging capabilities with a focus on security and efficiency. Whether for team collaboration, customer support, or social networking, ChatZo provides a reliable foundation for instant interactions.

## Steps to run the project

1. **Clone the repository**:
```bash
   git clone https://github.com/MUIabk/ChatZo.git
   cd ChatZo
```
2. **In root server directory you should run your go project**
```bash
  cd server
  go run cmd/main.go
```
3. **In root client directory you should run your next project**
```bash
  cd client
  npm i
  npm run dev
```

## API Reference

#### Local address
```bash
  http://127.0.0.1:8080
```
#### All endpoints

```http
   POST   /signup                   --> create new user
   POST   /login                    --> log into existing user
   GET    /logout                   --> log out of current user
   POST   /ws/createRoom            --> create room
   GET    /ws/joinRoom/:roomId      --> join room
   GET    /ws/getRooms              --> get all available rooms
   GET    /ws/getClients/:roomId    --> get all users in given room
```
