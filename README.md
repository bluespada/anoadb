# AnoaDB  
A fast and lightweight in-memory key-value store with TTL and encrypted persistence. Built with Rust and Tokio.  

## Overview  
AnoaDB is a key-value store designed to explore database internals, networking, and storage systems. It focuses on in-memory operations for speed while offering encrypted persistence for durability.  

This project is built for learning rather than production use. It covers low-level storage mechanisms, network communication, and concurrency models—essential concepts for anyone interested in database engineering.  

## Features  
- In-memory storage optimized for low-latency operations  
- TTL support for automatic key expiration  
- Encrypted persistence using JSON serialization  
- Asynchronous and multi-threaded, powered by Tokio  
- Dynamic type parsing for numbers, booleans, JSON, and plain strings  
- Lightweight UDP protocol for fast network communication  
- Multi-language SDKs for TypeScript, Java, and more  

## How It Works  

### Storage Layer  
- Uses a hashmap-based structure for in-memory storage  
- Supports persistence via encrypted JSON serialization  
- Values are stored as strings but interpreted dynamically when retrieved  

### Networking Layer  
- Uses UDP for fast, connectionless communication  
- A custom binary protocol (in progress) is being developed for efficiency  

### Concurrency Model  
- Built on Tokio’s async runtime to handle multiple operations in parallel  
- Uses multi-threading to distribute requests efficiently  

## Why AnoaDB?  
Many key-value stores exist, but AnoaDB is built for learning, not production. If you're interested in:  

- How databases store and retrieve data efficiently  
- Building high-performance networked applications  
- Asynchronous programming and concurrency in Rust  
- Creating your own key-value store from scratch  

This project provides a hands-on experience with real-world database concepts.  

## Note  
This project is intended for learning and experimentation. While fully functional, it is not designed for production use.  

## License  
MIT License – Open-source and freely available for modification and distribution.  
