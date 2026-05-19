# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
## CLIENT:
~~~
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
   msg=input("Client > ")
   s.send(msg.encode())
   print("Server > ",s.recv(1024).decode())

~~~
## SERVER:
~~~
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr = s. accept()
while True:
    ClientMessage=c.recv(1024).decode()
    c.send(ClientMessage.encode())
~~~

## OUPUT
<img width="952" height="491" alt="Screenshot 2026-05-20 051855" src="https://github.com/user-attachments/assets/24129558-c72c-4f91-b01d-a9ac5e18f957" />
<img width="949" height="530" alt="Screenshot 2026-05-20 051835" src="https://github.com/user-attachments/assets/9e5bbd73-0ccd-41b7-a4ed-6b4d9bdb3e0e" />




## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
