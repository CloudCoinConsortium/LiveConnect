# LiveConnect
This protocol allows persons to send and receive coins synchronistically. 


## Chat Server
There is an chat server that allows two people to connect to it. Once connected, the clients will start broadcasting info about their state and then transfer coins. 
All coins will be transfered in plain text. The Chat Sever must look at all text and change any # signs with the senders IP address.


## Protocol
This protocol is expandable.
It uses markeup tags to communicate the nature of each transaction.


Sequence of events: 

1. Sender decides that name of the IP, port number and the room number of the chat server. An encryption key is generated. 
2. Sender Finds its IP Address by doing an internet check
4. Client software generates a text file that can be read or given to the client. 
6. Sender connects to the chat room and a heart beat starts.<# Heartbeat>
7. Receiver finds its IP Address by doing an internet check
8. Receive connect to the chat room and a heart beat starts.<# Heartbeat>
9. Client and receiver can see each other's heartbeat and each others IP Address. they know that they have a connection.
10. Sender tells Receiver to empty mail box <# Empty In Box>
12. Receiver confirms <# Checking in Box>
12. Receiver makes sure inbox is empty. <# Box is Empty>
13. Sender specifies how much they want to send.<# Sending:3439>
14. Receiver Confirms <# Send:3439>
15. Sender Makes any change that is needed.<# Making Change>
16. Sender Joins coins to bigger coin if necessary<# Joining Coins>
17. Sender Finds Coins if lost <# Finding Change>
18. Sender Fixes Change if fracked <# Fixing Change>
19. Sender Puts coins in the Outbox <# Putting Coins in Outbox>
20. Sender runs detect <# Detecting coin authenticity>
21. Sender fixes coins <# Fixing Coins>
23. Receiver takes coins and puts them into inbox
. Receiver broadcasts that coins have been received
22. Receiver runs detect.
23. Receiver broadcasts that it is running detect.
24. Receiver broadcasts the results. 
25. If Good, Receiver runs POWN or PANG
26. Receiver broadcasts that money has changed
27. Transaction complete

