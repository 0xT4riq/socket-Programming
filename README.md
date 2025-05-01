# Socket Communication Example

This is a basic Python socket programming project that demonstrates how a client can communicate with a server using TCP sockets.

## 📂 Files

- `server.py`: Handles incoming client connections and prints received messages.
- `client.py`: Connects to the server and sends messages.

## 📌 Features

- Multi-threaded server to handle multiple clients.
- Custom message header for message length encoding.
- Graceful disconnection using a disconnect command.

## 🧰 Requirements

- Python 3.x

> No external libraries are needed — just the built-in `socket` and `threading` modules.

## 🚀 How to Run

### 1. Start the Server

Open a terminal and run:

```bash
python server.py

```

You should see:
```bash
[STARTING] Server is starting...
[LISTENING] Server is listening on <your IP address>

```
### 2. Run the Client

In a new terminal, run:
```bash
python client.py
```
This will send the message "Hello World!" to the server. The server will print:

```bash
[NEW CONNECTION] (<client IP>, <port>) connected.
[(<client IP>, <port>)] Hello World!

```