

## Python-chatroom

Python-chatroom is our first project at tek-up this application built using Python, with open-LDAP for authentication based on RabbitMQ to exchange message.




## Learning Goals 
•LDAP server:Manage user authentication.   
•Learning the fundamentals of encrypted message:creates certificattion, then signs them in order to verify their state and use authority server that accepts certification requests    
•Understanding RabbitMQ the exchange server and the  message-queueing
## Work plan
The creation of the application was divided in tow side.

Server :   

user registration:    

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

![Screenshot 2022-12-21 012906](https://user-images.githubusercontent.com/121107500/208949531-ed9b359c-baf8-43e9-bdb8-eb535358ba34.png)

![Screenshot 2022-12-21 131943](https://user-images.githubusercontent.com/121107500/208949893-1aff5111-496d-4565-a9fe-143e3c8c2058.png)

## Reliance

•RabbitMQ: Messaging Broker based on AMQP protocol.       
•OpenLDAP: is an implementation under ubuntu for LDAP protocol.  
•Pika: Rabbitmq python client.              
•Tkinter: Standard Python interface to the Tk GUI toolkit.


## Prerequisite

Open LDAP service 
 
$sudo apt -y install slapd ldap-utils 
$systemctl start ladp.service 

configure LDAP 


![Screenshot 2022-12-21 171049](https://user-images.githubusercontent.com/121107500/208950850-0966e7e2-af6f-4f0b-96ed-205e00465ff8.png)



Run RabbitMQ  
$ systemctl start rabbitmq-server

![Screenshot 2022-12-21 170312](https://user-images.githubusercontent.com/121107500/208950223-118fb5cd-c8cd-4fd6-8117-f83a2179dc9e.png)

