Single-Threaded Server-Client Application

This project demonstrates a simple Single-Threaded Server-Client communication model using Java Sockets. The server listens on a specified port, accepts connections from clients, and exchanges basic messages.

Features

Single-threaded server that handles one client connection at a time.

Basic communication between server and client using TCP (Transmission Control Protocol).

Demonstrates socket programming concepts in Java.

Tech Stack

Java

ServerSocket for server-side socket communication.

Socket for client-side socket communication.

PrintWriter and BufferedReader for input/output streams.

TCP Protocol for reliable communication.

Prerequisites

Java Development Kit (JDK) installed on your system.

An IDE like IntelliJ IDEA or a terminal with javac and java commands available.

Basic understanding of socket programming.

How to Run the Project

1. Clone the Repository

git clone https://github.com/GuptaChetan11/single-threaded-server-client.git
cd single-threaded-server-client

2. Compile the Java Files

Navigate to the directory containing the Server.java and Client.java files and compile them:

javac Server.java
javac Client.java

3. Run the Server

Start the server first to begin listening for client connections:

java Server

You should see:

Server is listening on port: 8010

4. Run the Client

Open another terminal or IDE instance and run the client:

java Client

You should see:

Received from server: Hello World from the server

On the server console, you’ll see:

Connected to /127.0.0.1:XXXXX

Project Files

Server.java:

Implements the server that listens on a specified port and handles client connections sequentially.

Client.java:

Implements the client that connects to the server and exchanges messages.

Key Concepts

Sockets:

Used for establishing a connection between the client and server.

TCP Protocol:

Ensures reliable, ordered delivery of data.

Streams:

InputStream and OutputStream are used for communication between client and server.

Single Thread:

The server processes one client connection at a time.

Example Output

Server Console

Server is listening on port: 8010
Connected to /127.0.0.1:50880

Client Console

Received from server: Hello World from the server

Troubleshooting

Common Issues

Client Not Connecting:

Ensure the server is running before starting the client.

Verify the server and client are using the same port.

No Output on Client Console:

Ensure the client reads and prints the response from the server.


Acknowledgments

Inspired by basic socket programming tutorials and Java documentation.

