# Decentralized File Storage System (Go)

A peer-to-peer distributed file storage system written in Go.  
It allows files to be uploaded, retrieved, removed, and broadcasted across multiple nodes with encryption support.  

## ✨ Features
- Custom TCP transport with handshake and error handling
- Peer-to-peer networking package for node discovery and communication
- File storage, retrieval, and deletion with directory management
- Message broadcasting across connected peers
- File encryption & decryption for data security
- Stream buffering for efficient data transfer
- Modular and extensible architecture

## 🛠️ Tech Stack
- **Language:** Go
- **Networking:** TCP, custom protocol
- **Security:** AES file encryption/decryption
- **Concurrency:** Goroutines, channels
- **Testing:** Go testing framework

## 🚀 Running the Project
```bash
# Start a storage node
go run cmd/main.go --port=5000

# Connect another node
go run cmd/main.go --port=5001 --peer=127.0.0.1:5000

# Upload a file
./client put myfile.txt

# Retrieve a file
./client get myfile.txt
