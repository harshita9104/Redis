# **Build Your Own Redis-like Server - Vanilla Node.js**

## **Introduction**

This project is a **custom-built in-memory key-value store** inspired by Redis, implemented entirely in **Vanilla Node.js**. It supports essential Redis commands, including **SET, GET, DEL, EXPIRE, TTL, INCR, DECR, and list operations**, as well as **data persistence using RDB (snapshotting) and AOF (Append-Only File logging)** for durability.

Through this project, you'll gain a **deep understanding of how Redis works under the hood**, covering **TCP servers, data structures, persistence mechanisms, and command execution**.

---

## **Features Implemented**

This project is structured in a step-by-step manner, ensuring a clear progression from basic server setup to advanced Redis functionalities:

### **1. Setting Up the Development Environment**

- Install **Node.js** and required dependencies.
- Initialize a **basic TCP server** using Node’s `net` module.
- Introduction to **Redis basics** and its working model.
- Setting up **Test-Driven Development (TDD)** for validation.

### **2. Handling Client Connections & Basic Commands**

- Implement a **TCP-based client-server connection**.
- Support for fundamental Redis-like commands:
  - `SET` - Store a key-value pair.
  - `GET` - Retrieve a value by key.
  - `DEL` - Delete a key-value pair.
  - `EXPIRE` - Set a time-to-live (TTL) for a key.

### **3. Implementing TTL and Atomic Operations**

- Handle **key expiration** using TTL.
- Support atomic operations:
  - `INCR` - Increment a numeric value.
  - `DECR` - Decrement a numeric value.

### **4. Handling Lists (Redis List Commands)**

- Implement Redis-like list operations:
  - `LPUSH` / `RPUSH` - Insert elements into a list (left/right).
  - `LPOP` / `RPOP` - Remove elements from a list (left/right).
  - `LRANGE` - Retrieve a range of elements from a list.

### **5. Adding Data Persistence with Snapshots (RDB)**

- Implement **RDB snapshotting**, allowing the server to persist data.
- Periodically **save the in-memory database to a file** for data recovery.

### **6. Implementing Append-Only File (AOF) for Durability**

- Introduce **AOF logging** to track all write operations.
- Replay AOF logs on restart to ensure **data durability**.
- Implement **configurable AOF flushing strategies**.

### **7. Project Recap and Future Improvements**

- Review of all implemented features.
- Potential improvements:
  - Implementing a **pub-sub messaging system**.
  - Optimizing data structures for efficiency.
  - Adding **support for advanced Redis commands**.

---
