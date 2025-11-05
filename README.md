# 🔐 SafeShare – Encrypted Multi-Client File Transfer System

## 📘 Project Overview

**SafeShare** is a **secure, command-line-based file sharing system** built in **C++**, designed to enable reliable and encrypted file transfer between multiple clients and a central server over TCP sockets.

It implements **AES encryption** to secure file contents during transmission, ensuring confidentiality and integrity.  
A **user authentication system** verifies login credentials before allowing access, while a **color-coded command-line interface** enhances user experience with intuitive visual cues.  
The **multithreaded server** can handle multiple clients simultaneously, displaying live transfer progress in real time.

---

## 🧠 Key Features

| Feature | Description |
|----------|-------------|
| 🔐 **AES Encryption** | All file data is encrypted using AES before transmission, ensuring secure communication. |
| 👤 **User Authentication** | Clients must log in with valid credentials (stored securely in a user file). |
| 🌈 **Color-Coded CLI** | Uses ANSI escape codes to show success (green), errors (red), warnings (yellow), and progress (cyan). |
| ⚡ **Multithreaded Server** | Handles multiple client connections simultaneously using `std::thread` or `pthread`. |
| 📤 **File Upload & Download** | Clients can securely send and receive files from the server. |
| 📊 **Progress Display** | Displays real-time upload/download percentage and connection status. |

---

## ⚙️ Tech Stack

- **Language:** C++  
- **Networking:** TCP Sockets (`sys/socket.h`, `arpa/inet.h`)  
- **Encryption:** OpenSSL (AES-256-CBC)  
- **Threading:** `std::thread` / POSIX Threads  
- **Interface:** ANSI color-coded terminal UI  
- **Storage:** Text-based user database (`users.txt`)

---

## 🪜 Build & Run Instructions

### 🧰 Prerequisites
- Linux environment (Ubuntu recommended)
- OpenSSL library installed  
  ```bash
  sudo apt-get install libssl-dev
