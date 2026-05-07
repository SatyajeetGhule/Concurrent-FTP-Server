# Concurrent FTP Server

A Concurrent FTP Server implemented in C using Linux System Programming concepts. This project allows multiple clients to connect and download files simultaneously using TCP socket programming and fork()-based concurrency.

## 🚀 Features

* Multi-client support using `fork()`
* Reliable file transfer over TCP
* Custom protocol design (Header + Payload)
* Chunk-based file transmission
* Linux system calls for networking and file handling
* Proper error handling and validation

## 🛠️ Technologies Used

* C Programming
* Linux System Programming
* TCP/IP Socket Programming

## 📚 Concepts Covered

* Client-Server Architecture
* Concurrent Programming
* Process Management
* Socket Programming
* File System Operations
* Protocol Design

## ⚙️ System Calls Used

### File Subsystem

* `open()`
* `read()`
* `write()`
* `close()`
* `stat()`

### Network Subsystem

* `socket()`
* `bind()`
* `listen()`
* `accept()`
* `connect()`
* `send()`
* `recv()`

### Process Subsystem

* `fork()`
* `wait()`
* `exit()`

## 📦 How It Works

1. Server starts listening on a TCP port.
2. Client connects and requests a file.
3. Server creates a child process using `fork()`.
4. Server sends file metadata (header).
5. File is transferred in chunks.
6. Multiple clients can download files concurrently.

## 🎯 Learning Outcomes

* Deep understanding of Linux networking
* Hands-on experience with concurrent servers
* Practical TCP/IP socket programming
* Understanding of process-based concurrency
* Experience with protocol-driven communication

## ▶️ Build & Run

### Compile

```bash
gcc server.c -o server
gcc client.c -o client
```

### Run Server

```bash
./server
```

### Run Client

```bash
./client
```

## 📌 Future Improvements

* File upload support
* Authentication system
* Multi-threading support
* epoll/select based scalability
* Secure encrypted transfer
* Logging system

## 👨‍💻 Author

Satyajeet Ghule
