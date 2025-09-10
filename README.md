# ⚡ Client–Server HTTP (C++)

This project demonstrates communication between a **client and a server using the HTTP protocol** written in **C++**.  
The project also includes an example of serving simple resources – battery icons that can be delivered by the server to the client.

---

## ⚙️ Requirements

- **C++ compiler** (g++, clang++)
- **Linux/Unix environment** (the project uses sockets)
- Optional: Web browser or `curl` for testing HTTP responses

---

## 🔨 Build

To compile both the client and the server, simply run:

```bash
make
```
This will produce two binaries: server and client.

You can also compile manually:
```bash
g++ server.cpp -o server
g++ client.cpp -o client
```

🚀 Run

1. Start the server (e.g., on port 8080):
```bash
./server 8080
```
2. Start the client (connects to the server):
```bash
./client 127.0.0.1 8080
```

3. The client sends an HTTP request, and the server responds with an HTTP response.
The server can also provide static resources such as battery icons (battery-xxx.png).

## 🌐 Functionality

- The server listens for client connections and processes simple HTTP requests.

- The client sends HTTP requests and receives responses.

- You can test the server using curl or a web browser:
```bash
curl http://127.0.0.1:8080/
```
- Battery icons are included as example static content that the server can serve.


## 🧑‍💻 Author

Created by **Adam Kuchár**  