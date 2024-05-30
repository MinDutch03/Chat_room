# Simple Chat Application

Contained within this repository is a simple chat application implemented in Java, utilizing the TCP protocol. The application comprises a server and a client component.

## Server :computer:
The server manages incoming client connections and facilitates communication between them. It supports message exchange, nickname customization, and graceful chat exits. Implemented as a multithreaded system, it efficiently handles concurrent client connections.

### How to Run the Server :gear:
Follow these steps to run the server:

* Run the `Server.java` file.

To initiate the server, execute the Server.java file.

The server initializes and begins listening for client connections on port 1234.

## Client :
The client interface is command-line based and connects to the server, enabling users to participate in chat interactions. Users can exchange messages, modify their nicknames, and exit the chat seamlessly.

### How to Run the Client :gear:
To launch the client, execute the Client.java file.

By default, the client connects to the server hosted on 127.0.0.1 (localhost) at port 1234. Adjustments to the server address can be made within the Client class if necessary.

## Usage :bulb:
- Upon connecting, clients are prompted to set a nickname.
- Messages can be sent by typing and pressing Enter.
- Nicknames can be changed using the "/change_nick" command followed by the desired name (e.g., "/change_nick <NewNickname>").
- When a client types "bye", they exit the chat. Once all clients have left, the server terminates automatically.

## Features :rocket:
- The server supports concurrent connections from multiple clients through multithreading.
- Clients can personalize their identities by modifying their nicknames.
- Client disconnections are handled gracefully to maintain chat stability.
