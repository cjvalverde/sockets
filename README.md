# sockets

**Version 1.0.0**

Code for two simple server/client implementations to use SOCKETS and PICKLE.

---

## Contents

- server.py
- client.py
- server_objects.py
- client_objects.py
- README.md

---

## How it works


- Simple server/client implementation (server.py and client.py) using sockets AF_INET / SOCK_STREAM. Server sends a string of text to the client with a fixed length header (10 characters) which contains the lenth of the message. The client  uses this number to stop waiting when message is fully received.
- Simiar to the simple server/client implementation (server_objects.py and client_objects.py), but using the module PICKLE to enable sending of any python objects (tested with a dictionary). The server uses PICKLE to convert an object in a string of characters to send. The client uses PICKLE to converts the received string back into an object.

To test the simple server, clone this repository and run server.py and then client.py on any IDE (like Pycharm) or in separate cmd windows from the project folder location executing for example "py server.py".

To test the server that sends objects, clone this repository and run server_objects.py and then client_objects.py on any IDE (like Pycharm) or in separate cmd windows from the project folder location executing for example "py server.py".
  
---

## Required modules

- sockets
- tickle
- time

---

## Contributors

- Carlos Valverde <carlos_valverdeb@hotmail.com>

---
## Licence and copyright

© Carlos Valverde