# Multithreaded Chat Room


ABOUT</br>
This project was created as part of open projects floated by ACM, IIT Roorkee Chapter.
It is a multithreaded client/server ChatServer based on console which uses C++ Socket programming. A server listens for connection requests from clients across the network or even from the same machine. After connecting to the server, the client gets to choose his/her username on the chat room. The clients are added on multiple threads to execute concurrently. Using many threads would lead to a situation where two threads are accessing the same code or the same shared variable and there is a possibility of wrong output. To tackle this situation mutex locks are used to allow only one thread to access the shared code and do the necessary changes and synchronize all the threads.

INSTRUCTIONS:

To compile run the following commands in command line(terminal) on linux based system:

g++ server.cpp -lpthread -o server</br>
g++ client.cpp -lpthread -o client</br>

SERVER SIDE:-

Run the following command on terminal to start server - ./server

CLIENT SIDE:-

Run the following command on terminal to start client - ./client
Enter the username
Chat box starts after a username is entered.
Enter the chat text 


Note-: To simulate multiple users, open up a new command line window and type ./client.
