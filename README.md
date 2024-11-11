# TCP Chat Application 

This project implements a multi-client chat application in Python. The server can handle multiple clients, allowing them to send messages to each other in real time. Additionally, the application includes administrator privileges for enhanced chatroom management.

## Features
- **Real-time messaging**: Clients can send and receive messages instantly.
- **Admin controls**: Users with the name "admin" can kick or ban other users from the chat room.
- **Persistent bans**: Banned users are stored in `bans.txt` to prevent re-entry.

## Usage
1. Start the server using `server.py`.
2. Run `client.py` for each client connection.
3. Use `/kick <nickname>` and `/ban <nickname>` commands as admin to manage users.

**Note**: Default admin password is `adminpass`. The server IP and port are set to `127.0.0.1` and `55556` respectively.





## Usage and Functionality

The **Chat Application** is designed to allow multiple users to connect and communicate in real time through a central server. To start, run `server.py` on the host machine, which will keep listening for incoming client connections. Users connect by running `client.py`, which prompts them to choose a nickname. The nickname "admin" is reserved for administrators, who can execute specific commands such as `/kick <nickname>` to remove users and `/ban <nickname>` to permanently ban them from reconnecting. Each client can see messages sent by others, fostering a group chat environment. Additionally, banned users' nicknames are saved in `bans.txt` to ensure they cannot rejoin even after restarting the server. 