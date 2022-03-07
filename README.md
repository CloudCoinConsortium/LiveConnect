# LiveConnect
This protocol allows persons to send and receive coins synchronistically. 


## Chat Server
There is an chat server that allows two people to connect to it. Once connected, the clients will start broadcasting info about their state and then transfer coins. 
All coins will be transfered in encrypted bytes. But the commands will be clear . The Chat Sever must look at all text and change any # signs with the senders IP address.


## Protocol
This protocol is expandable.
It uses markeup tags to communicate the nature of each transaction.


Sequence of events: 
Note: The sender and the receiver wil have hidden wallets called "Sender" and "Receiver"
1. Sender decides that name of the IP, port number and the room number of the chat server. An encryption key is generated. 
2. Client software generates a text file that can be read or given to the client. This Text File has the connection Information 
3. Sender connects to the chat room and a heart beat starts.<# Heartbeat> The IP Addresss are now show by the chat server. 
4. Receive connect to the chat room and a heart beat starts.<# Heartbeat>
5. Client and receiver can see each other's heartbeat and each others IP Address. they know that they are told they have a connection. 
6. Sender tells Receiver to empty Import and Export folders<# Empty_Import_Export>
7. Receiver checks its "Receiver" wallet's inbox and confirms <# Import_Export_Empty>
8. Sender specifies how much they want to send.<# 3439>
9. Receiver Confirms <# 3439>
10. Sender Makes any change that is needed.<# Making_Change>
11. Sender Joins coins to bigger coin if necessary<# Joining_Coins>
12. Sender Finds Change if lost <# Finding_Change>
13. Sender Fixes Change if fracked <# Fixing_Change>
14. Sender moves coins to the Bank folder of the hidden Sender Wallet.<# Moving_Coins_To_Sender>
15. Sender runs health check <# Detecting_Coin_authenticity>
16. Sender Fixes Coins if fracked <# Fixing_Coins>
17. Sender Puts coins in the Export <# Putting_Coins_in_Export>
18. Sender asks Receiver if ready <# Ready_To_Send_Coins>
19. Receiver replies <# Ready_To_Receive>
20. Sender sends coins and puts them in the Sent Folder. <# coin> binary code </coin><# coin>binary code </coin>
21. Receiver takes coins and puts them into Import folder in their hidden receive wallet. 
22  Receiver broadcasts that coins have been received <# Received>
23. Receiver runs pown <# Powning_Coins>
24. Receiver sends receipt <# receipt>  </receipt>
25. Sender sees receipt. 

```javascript

{
"from": "192.168.1.54",
"Message Number": 1,
"Message_Details": "dfsdfs",
}


```


Protocol
Message Number | Details | Message Name
---|---|---
1 | None | Heartbeat
2 | None | Empty_Import_Export
3 | None | Import_Export_Empty
4 | An Integer | Money to be Sent
5 | None | Making_Change
6 | None | Joining_Coins
7 | None | Finding_Change
8 | None | Moving_Coins_To_Sender
9 | None | Detecting_Coin_authenticity
10 | None | Fixing_Coins
11 | None | Putting_Coins_in_Export
12 | None | Encrypting Coins
13 | None | Ready_To_Receive
24 | Base64 Encrypted | Coins 
14 | None | Received
15 | None | Decrypting_Coins
16 | None | Powning_Coins
17 | The Receipt base 64 | receipt
18 | None | Confirming Change of Ownership
19 | None | Coins confirmed. 







