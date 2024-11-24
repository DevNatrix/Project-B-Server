# Project-B-Server
This is a C++ game server that uses both UDP and TCP to handle different types of data

UDP is used for things like player movement and game states that are updated frequently. It’s faster and saves bandwidth by not resending lost messages.
TCP handles important events and messages that need to be delivered reliably.
The server is mostly event-based but also works like a "phone line," processing specific messages and simply forwarding the rest. It’s designed to be lightweight and efficient, so it can run on devices like a Raspberry Pi while supporting a high number of players.
