# 📝 Tutorial & Exercise 10 📝

**Student Details:**

| Attribute | Information                |
|-----------|----------------------------|
| Name      | Andika Pramudya Wardana   |
| Student ID| 2206046645                 |
| Class     | Advanced Programming KKI   |

---

<details>
<summary>Module 10: High-Level Networking Part 2</summary>

## Questions and Answers

### -> Reflection

#### Experiment 2.1: Original code, and how it run
**Result:** 
```rust 
    listening on port 2000
    New connection from 127.0.0.1:62821
    From client 127.0.0.1:62821 "hello"
    New connection from 127.0.0.1:62826
    From client 127.0.0.1:62826 "my name is Andika"
    New connection from 127.0.0.1:62829
    From client 127.0.0.1:62829 "my npm is 2206046645"
```
    First, I compile the server by running "cargo build --bin server". Next, I run the server with "cargo run --bin server". Once the server is running, it will output messages to the terminal indicating that it's listening on a particular port (in this case, port 2000).

    Next, after the server runs, i compile the client by running "cargo build --bin client". Next, I run the clients 3 times in different terminal by running "cargo run --bin client" for each terminal

    Last, after the server & client are running, i look into the server's terminal and see that it output on which port the server is listening to and it also output a new connection from 3 new client (IP address and port number combination) including each messages i input to each client's terminal before.

#### Experiment 2.2: Modifying port
    This code sets up a chat system where one computer (the server) listens for messages from other computers (clients) using a technology called WebSocket. Originally, the server listened on a particular "door" called port 2000, but we changed it to port 8080. When a client wants to join the chat, it connects to the server's address, which includes the port number (now 8080 instead of 2000). Once connected, clients can send messages to the server, which then shares those messages with all other connected clients. This way, everyone can chat with each other in real-time. We use a special tool (a Rust crate) called tokio_websockets to handle all the complicated communication stuff behind the scenes.

