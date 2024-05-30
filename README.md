# Simple Chat Application

This repository contains a straightforward Java-based chat application using the TCP protocol, consisting of a server and a client.

## Server :computer:
The server is responsible for handling incoming client connections and facilitating communication between clients. It allows clients to send messages, change their nicknames, and gracefully quit the chat. The server is a multithreaded application, capable of handling multiple client connections simultaneously.

### How to Run the Server :gear:
Follow these steps to run the server:

* Run the `Server.java` file.


The server will start listening on port 1234 for incoming client connections.

## Client :
The client is a command-line application that connects to the server, enabling users to send and receive messages in a chat room. Clients can also change their nicknames and quit the chat gracefully.

### How to Run the Client :gear:
Follow these steps to run the client:

* Run the `Client.java` file.

The client will connect to the server running on `127.0.0.1` (localhost) on port 1234 by default. You can change the server address in the `Client` class if needed.

## Usage :bulb:
- When a client connects, they will be prompted to enter a nickname.
- Clients can send messages to the chat by typing their messages and pressing Enter.
- To change their nickname, clients can use the "/nick" command followed by the desired nickname (e.g., "/nick NewNickname").
- To quit the chat, clients can use the "/quit" command.

## Features :rocket:
- Multithreaded server that can handle multiple client connections simultaneously.
- Ability for clients to change their nicknames to distinguish themselves in the chat.
- Graceful handling of client disconnections.
