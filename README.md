
## Python-chatroom

Python-chatroom is our first project at tek-up this application built using Python, with open-LDAP for authentication based on RabbitMQ to exchange message.




## Learning Goals 
•LDAP server:Manage user authentication.   
•Learning the fundamentals of encrypted message:creates certificattion, then signs them in order to verify their state and use authority server that accepts certification requests    
•Understanding RabbitMQ the exchange server and the  message-queueing
## Work plan
The creation of the application was divided in tow side.

Server :   

User registration:    

•Add a new user to Active Directory via LDAP  
•Get certificate through authority server  
•Initiate communication with the Chat/Rabbitmq server

Login User:  

•Check Active Directory users via LDAP  
•Validate signature via authority server
•chat Encryption/decryption of messages exchanged between clients

Customer :

•Enter access data (first time)  
•Login block authentication (transfer)     
•It uses RSA technology to encrypt/decrypt all messages sent between client       
•Disconnect 

![Screenshot 2022-12-21 012906](https://user-images.githubusercontent.com/121107500/208904805-4cc3ece1-1757-4a68-a5ac-c77d07bdceba.png)




## Reliance

•RabbitMQ: Messaging Broker based on AMQP protocol.       
•OpenLDAP: is an implementation under ubuntu for LDAP protocol.  
•Pika: Rabbitmq python client.     
•Tkinter: Standard Python interface to the Tk GUI toolkit.

![Screenshot 2022-12-21 131943](https://user-images.githubusercontent.com/121107500/208905015-a75a95b2-5828-4ae2-9bb7-2f7c54452c86.png)


