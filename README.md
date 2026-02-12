💬 TCP Chatroom Application

A multi-client chatroom application built using Python Socket Programming (TCP).
This project demonstrates real-time communication between multiple clients connected to a central server.

📌 Project Overview

The TCP Chatroom allows multiple users to:

Connect to a central server

Send and receive messages in real-time

Communicate in a shared chat environment

The system uses:

TCP protocol

Client-Server architecture

Multithreading for handling multiple clients

🏗️ Architecture
            ┌─────────────┐
            │   Server    │
            └──────┬──────┘
                   │
        ┌──────────┼──────────┐
        │          │          │
     Client 1   Client 2   Client 3


The Server listens for incoming connections.

Multiple Clients connect to the server.

Messages from one client are broadcast to all connected clients.

⚙️ Features

Multi-client support

Real-time messaging

Broadcast messaging

Thread-based client handling

Simple and lightweight design

Runs in terminal/command prompt

🛠️ Tech Stack

Python 3

Socket Programming

Threading Module

📂 Project Structure
TCP-CHATROOM/
│
├── server.py
├── client.py
└── README.md

🚀 How to Run
1️⃣ Clone the repository
git clone https://github.com/your-username/TCP-CHATROOM.git
cd TCP-CHATROOM

2️⃣ Run the Server
python server.py


The server will start listening for connections.

3️⃣ Run the Client (Open Multiple Terminals)
python client.py


Each client can now send and receive messages.

🔍 How It Works
Server:

Creates a TCP socket

Binds to a host and port

Listens for incoming connections

Spawns a new thread for each connected client

Broadcasts received messages to all clients

Client:

Connects to the server

Sends messages to server

Listens for broadcast messages

Displays incoming messages in real-time

📡 Networking Concepts Used

TCP Protocol

Socket Binding

Port Communication

Multithreading

Client-Server Model

🔐 Possible Improvements

Add username authentication

Private messaging

GUI version (Tkinter / PyQt)

Message encryption

Chat history storage

Deployment over LAN/Internet

📘 Learning Outcomes

This project helps in understanding:

Low-level network programming

Concurrent client handling

Thread synchronization basics

Real-time communication systems
