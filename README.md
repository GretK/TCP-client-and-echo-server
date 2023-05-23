# TCP-client-and-echo-server
Practice developing simple TCP client and TCP server to gain experience in creating network applications and to realize the importance of security and reliability in such systems.

**Project task:**
Create a simple TCP server that receives a string from a client (in chunks of 1 KB) and echoes it back (echo server).
The server should output informative messages (with explanations) to the console when any of the following events occur:

- Server startup;
- Start listening on the port;
- Client connection;
- Receiving data from the client;
- Sending data to the client;
- Client disconnection;
- Server shutdown;

Write a simple TCP client that establishes a connection with the server, reads a string from standard input, and sends it to the server.
The client should output informative messages (with explanations) to the console when any of the following events occur:

- Connection to the server;
- Disconnection from the server;
- Sending data to the server;
- Receiving data from the server.

**Additions:**

1. Modify the server code to continue listening on the same port even after a client disconnects, allowing for reconnection.
2. Modify the client and server code to prompt the user for the port number and host name (for the client).
3. Implement secure input of data and default values.
4. Modify the server code to output all informative messages to a dedicated log file instead of the console.
5. Modify the server code to automatically change the port number if it is already in use. The server should output the port number it is listening on to the console.
6. Implement an identification server. The server should accept connections from clients and check if the client is already known based on its IP address. If known, the server should greet the client by name. If unknown, the server should prompt the user for a name and record it in a file.
7. Implement an authentication server. Similar to the previous task, but along with the user's name, the server also tracks and verifies passwords.
8. Implement secure storage of passwords.
9. Implement session maintenance based on a token similar to cookies.
10. Write auxiliary functions to send and receive text messages over the socket. The sending function should prepend the message with a fixed-length header containing information about the message length. The receiving function should read the message considering the header.
11. Implement string-to-byte array conversion and vice versa within these functions.
12. Implement these functions as an inherited extension of the socket class from the socket library.
13. Enhance the client and server code to allow sending multiple messages to each other in response to previous messages.
