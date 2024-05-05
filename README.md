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

