# SSH (Secure Socket Shell)

## Table of Contents
- Introduction


### About SSH? A Beginner's guide to Secure SSH
- A Secure Shell, or Secure Socket Shell, is a network protocol that allows devices to achieve two important things: communicate and share data. Additionally, the SSH protocol also encrypts data, making it ideal for unsecured networks.

### What is SSH Exactly??


As a term, Secure Socket Shell, defines both a cryptographic network protocol and the programs that enable it to work.

> SSH enables network administrators to access a computer via an unsecured network in a safe manner. It ensures a secure connection that allows it to operate and manage remote computers without worrying about the safety of shared data.  

To achieve this, the SSH protocol does not only provide encryption with the help of a secure channel but also strong password authentication and public-key authentication.

The SSH protocol and SSH keys – access credentials within the protocol – secure millions of file transfers, automated functions and upkeep sessions per day. 

Continue reading if you wish to learn more about SSH servers and the client programs that enable reaching them. As well as the primary use cases of the SSH protocol and its vulnerabilities.


### How does SSH work?



SSH uses the client-server model to connect the application and the server, or the location where the session is shown and the place where it’s actually running.

In other words, the SSH clients contact SSH servers to begin the connection setup process. An SSH server sends its public key, and with the help of public-key cryptography, the client tries to verify the server’s identity. 

Once this is over, the SSH protocol starts using strong symmetric encryption protocols and hashing algorithms to establish privacy and secure file transfers. This is how data is exchanged between client and server safely.

SSH client and server do this with the help of various encryption methods, but the most common ones are Blowfish and the Advanced Encryption Standard. 

Blowfish is the oldest symmetric encryption algorithm. However, the Advanced Encryption Standard, developed by the National Institute of Standards and Technology, is used more widely. 



SSH also works similarly to a typical Virtual Private Network (VPN). A VPN also creates an encrypted tunnel for secure communication. The only difference is that a VPN doesn’t use the client-server model but, instead, a secure connection between your device and the VPN server.

It is also important to note that the SSH secure connection works differently on different operating systems:

    On Mac and Linux – via Terminal
    On Windows – via an installed SSH client 

The client-server relationship can be tricky to understand. So, let’s delve into how both SSH servers and SSH clients work. 





