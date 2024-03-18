Attack is the best defense

For this project, we expect you to look at these concepts:

Network basics
Docker

Background Context
This project is NOT mandatory at all. It is 100% optional. Doing any part of this project will add a project grade of over 100% to your average. Your score won’t get hurt if you don’t do it, but if your current average is greater than your score on this project, your average might go down. Have fun!

Resources
Read or watch:

Network sniffing
ARP spoofing
Connect to SendGrid’s SMTP relay using telnet
What is Docker and why is it popular?
Dictionary attack

Tasks
0. ARP spoofing and sniffing unencrypted traffic
Security is a vast topic, and network security is an important part of it. A lot of very sensitive information goes over networks that are used by many people, and some people might have bad intentions. Traffic going through a network can be intercepted by a malicious machine pretending to be another network device. Once the traffic is redirected to the malicious machine, the hacker can keep a copy of it and analyze it for potential interesting information. It is important to note that the traffic must then be forwarded to the actual device it was supposed to go (so that users and the system keep going as if nothing happened).

1. Dictionary attack
Password-based authentication systems can be easily broken by using a dictionary attack (you’ll have to find your own password dictionary). Let’s try it on an SSH account.

Install Docker on your machine Ubuntu
Pull and run the Docker image sylvainkalache/264-1 with the command docker run -p 2222:22 -d -ti sylvainkalache/264-1
Find a password dictionary (you might need multiple of them)
Install and use hydra to try to brute force the account sylvain via SSH on the Docker container
Because the Docker container is running locally, hydra should access the SSH account via IP 127.0.0.1 and port 2222
Hint: the password is 11 characters long
Once you found the password, share it in your answer file.
