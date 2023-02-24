# Secure Shell Protocol (SSH)

## Table of Contents



Secure shell is a common term often used when studying computer networks. In simple terms, **SSH secure shell refers to a secured network protocol that helps access remote computers securely in a network. However, it is much more complicated than it sounds.**

> So in this blog, we will study all about secure shell protocol. Also, we will explore its working, its concepts, and the mechanisms it leverages for safe remote access. Let us start!

### What is a Secure Shell?

**SSH** in computer networks refers to a remote administration protocol that enables users, especially system administrators, to access, manage, and modify the remote servers over an unsecured network.

**SSH** facilitates public key authentication and strong password authentication for servers. It is also used to communicate between two computers that use encrypted data over an open network or the internet.

Additionally, system administrators widely use secure shells to log in to a different computer system over a network. They utilize it to execute commands and transfer files from one system to another.

**SSH** is a common term used both for cryptographic network protocol and the suite of utilities that implement the protocol. Secure shell usually leverages a client-server model that connects an SSH secure shell client application to an SSH server.

SSH is a highly versatile protocol and can also be used to build secure tunnels for other application protocols.

## Why Do We Need SSH in Computer Networks?

> The need for the secure shell protocol goes back to its beginning in 1995, when it was designed to solve security issues faced by unsecured remote access protocols like Telnet, rlogin, and rsh.

> Telnet was the most used protocol back then used to transmit and​ receive messages over a network. However, the biggest challenge with Telnet was that it was highly insecure.

As the data was transmitted to multiple networks, there was a chance of data being intercepted and manipulated before reaching the target machine. At those times, communication used to happen in plain text without encryption.

Hence, intercepting the network and stealing the information was extremely simple. So, the SSH secure shell protocol was devised with an encryption mechanism that could save the data from being wrongly modified.

Another reason why SSH is important in current times is because of the evolved technology. **Today the market is of cloud servers. Most enterprises prefer using cloud servers for their websites. SSH enables network administrators to perform several tasks on cloud servers.**


SSH is generally used for:

    Setting up a web server for the client’s website.
    Deploying source code to a production server.
    
    
** How Does Secure Shell Protocol Work?

Secure shell protocol leverages a client-server architecture to establish secure network communication. It connects an SSH secure shell client with a secure ssh server. The SSH server is by default programmed to listen to the standard TCP port 22. Hence, SSH uses this port to initiate communication with other remote systems.

To authenticate the client and the server, **SSH utilizes the public-key cryptography technique.** The protocol uses hashing algorithms and strong symmetric encryption to exchange messages between client and server. It provides a great way to ensure data privacy and data integrity.

Mostly, Linux is used for running the SSH protocol because of its durability and security. However, if you are using a Windows-based system, you will need a SSH secure shell client to access SSH connections.

