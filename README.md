# AnoaDB  
*A fast and lightweight in-memory key-value store with TTL and encrypted persistence. Built with Rust and Tokio.*  

## Overview  
AnoaDB is a simple yet powerful key-value store designed for **understanding database internals, networking, and storage systems**. Unlike traditional databases, it focuses on in-memory operations for speed while offering **encrypted persistence** to ensure data durability.  

This project is built to **explore** rather than replace production-ready solutions. It covers **low-level storage mechanisms, network communication, and concurrency models**—all essential for anyone interested in **database engineering**.  

## Features  
- **In-Memory Storage** – Optimized for low-latency read/write operations.  
- **TTL Support** – Automatically removes expired keys.  
- **Encrypted Persistence** – Securely stores data in an encrypted JSON format.  
- **Asynchronous & Multi-Threaded** – Built with Tokio for concurrent processing.  
- **Dynamic Type Parsing** – Interprets stored values as numbers, booleans, JSON objects, or plain strings.  
- **Lightweight UDP Protocol** – Uses minimal overhead for fast network communication.  
- **Multi-Language SDKs** – Supports integration with TypeScript, Java, and more.  

## How It Works  

### **1. Storage Layer**  
- Implements an **in-memory key-value store** using a **hashmap-based structure**.  
- Supports **persistence via encrypted JSON serialization**.  
- Values are stored as strings but can be **interpreted dynamically** when retrieved.  

### **2. Networking Layer**  
- Uses **UDP** for fast, connectionless communication.  
- A **custom binary protocol** (in progress) is being developed for better efficiency.  

### **3. Concurrency Model**  
- Built on **Tokio’s async runtime** to handle multiple operations in parallel.  
- Uses **multi-threading** to distribute requests efficiently.  

## Why AnoaDB?  
Many key-value stores exist, but AnoaDB is built for **learning, not production**. If you're interested in:  

- **How databases store and retrieve data efficiently**  
- **Building high-performance networked applications**  
- **Asynchronous programming and concurrency in Rust**  
- **Creating your own key-value store from scratch**  

Then this project provides a **hands-on experience** with real-world database concepts.  

## Note  
This project is intended for **learning and experimentation**. While fully functional, it is **not designed for production use**.  

## License  
**MIT License** – Open-source and freely available for modification and distribution.  
