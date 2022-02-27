# LiveConnect
This protocol allows persons to send and receive coins synchronistically. 


## Chat Server
There is an chat server that allows two people to connect to it. Once connected, the clients will start broadcasting info about their state and then transfer coins. 
All coins will be transfered in plain text. The Chat Sever must look at all text and change any # signs with the senders IP address.


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
from:'192.168.1.54',


}


```


Protocol
Sequence Number | Character | Text
---|---|---
1 | A | Heartbeat
2 | B | Empty_Import_Export
2 | B | Import_Export_Empty
2 | B | 3439
2 | B | Making_Change
2 | B | Joining_Coins
2 | B | Finding_Change
2 | B | Moving_Coins_To_Sender
2 | B | Detecting_Coin_authenticity
2 | B | Fixing_Coins
2 | B | Putting_Coins_in_Export
2 | B | Encrypting Coins
2 | B | Ready_To_Receive
2 | B | Received
2 | B | Decrypting_Coins
2 | B | Powning_Coins
2 | B | receipt
2 | B | Confirming Change of Ownership
<






