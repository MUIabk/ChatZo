## Technology list in this project

in back-end:

in front-end:

## How to run

In root server directory you should run your go project
```bash
  go run cmd/main.go
```
In root client directory you should run your next project
```bash
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
