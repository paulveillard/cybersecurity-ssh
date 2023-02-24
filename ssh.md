# Secure Shell Protocol (SSH)

## Table of Contents
- [What is a Secure Shell]()


Secure shell is a common term often used when studying computer networks. In simple terms, **SSH secure shell refers to a secured network protocol that helps access remote computers securely in a network. However, it is much more complicated than it sounds.**

![ssh-intro](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-tutorial-how-does-ssh-work.png)

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


### The Working Operation of SSH

![ssh-operations](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-meaning.png)

SSH sessions generally have only two operations:

#### 1. Authentication

The SSH servers need to authenticate clients before they can access the network. To authenticate clients, two methods are usually used:

    Password-Based: In this method, the SSH server uses a password to authenticate the clients. It is one of the most basic methods used for authentication purposes. However, this method is not very secure and can be bypassed using brute force attacks. 

    Key-Based: It is a more reliable and secure way to authenticate clients. This method generates and matches SSH key pairs to authenticate users and establish a secure connection. 

#### 2. Command Execution

The next task of the secure shell protocol is to access the remote server using different commands. Mac and Linux users have the benefit of directly using the terminal to execute SSH commands.

However, a third-party terminal emulator client needs to be installed for Windows users to run the commands. The most popular and widely used SSH secure shell client is PuTTY.

##### How to Connect?

For connecting to a remote server using SSH, you must have the details of:

    server host
    user name

The basic SSH command is:

> $ ssh <user-name> @ <host> -p <port-no>

Where:

    The username is the remote machine you are trying to connect to.
    The host is either a domain name or an IP address.

On successfully entering these credentials, you will log on to the remote system server. There you can use the terminal of that system to execute commands and do the needful operations.
    
    
### Glancing at the Features of SSH

SSH secure shell has multiple features that make it essential in computer networks. Some of its features are as follows:

    
### Secure Remote Logins

The fundamental feature of the SSH secure shell protocol is to provide secure login access to a remote system over open networks. Your username and password are encrypted on the local machine before establishing a connection.

The client then uses this encrypted connection to authenticate you to the remote system’s SSH server. The entire login session remains encrypted in this mechanism
    
    
### Secure File Transfer

Another great feature for which SSH is loved and used by thousands of network administrators is its ability to securely transfer a file with quick speed. You literally need to type a single copy command along with the filename and its source, and the file is ready to get transferred. The file gets encrypted before the transfer and automatically decrypts after the transfer.

Here is the command to transfer a file from one system to another remote system:

 $ scp myfile metoo@secondaccount.com

### Secure Remote Command Execution

System administrators often need to run the same command on different computers. However, to save themselves from this monotonous task, secure shell offers a way to securely execute the command for different computers in one go.

Here is the command used to do it:

#!/bin/sh

for machine in 1 2 3 4 (1,2,3,4 are the machine names)

do

ssh $machine /usr/bin/w

done
    
### Keys and Agents

Remembering multiple passwords for different networks and computer systems is a tough task. That is why the SSH secure shell makes use of keys for its authentication mechanisms. Leveraging the keys and a program known as an authentication agent, secure shell protocol authenticates you to all your computer accounts securely in one go.

You just need to enter all the key files once into your remote system accounts. Then every time you need to access a system, you can invoke the ssh-agent program using the command line that helps you to access the remote system without asking for authentication.
    
    
### Access Control

SSH also allows its users to permit another person to use their personal account to access remote computers. However, the other person may get only limited access to certain functionalities.

Moreover, your password or the keys does not get exposed to the user you are lending your system to. It is a highly beneficial feature that eases the workflow for network and system administrators. 

### Port Forwarding

It is a technique in which a TCP/IP connection can be passed through a secure shell connection to secure data transmission. This process is also known as tunneling in computer networks. It is mostly used when a network firewall blocks incoming connections to the system ports.

It occurs mostly while operating your office systems. To bypass the firewall, the SSH protocol can establish a secure tunnel on an arbitrary local TCP port and offer transmission of data.
    
### How Secure is SSH?

In general, SSH secure shell is considered one of the safest protocols for remote network communication. However, SSH, too, has its drawbacks. Brute force attacks can be made when using passwords to establish a connection using SSH. The brute force attack involves using common usernames and passwords to access the SSH servers and the root account.

Conversely, SSH keys are a more secure way to authenticate. Unfortunately, if your SSH key management routine is poor, hackers can still manage to gain access to the keys in your system.

Besides, their misuse can be highly disastrous as it can lead to access to privileged information such as databases, routers, payment systems, etc.

Apart from it, another potential security weakness of SSH is Exposed SSH ports. Some malware programs can attack the exposed ports and use them to breach the local network.

However, all these scenarios are not so common and easy to implement. But you should always take the right measures and be aware of your networks to ensure the best security for your system.
    
    
 ### Conclusion

[SSH](https://cheapsslweb.com/blog/an-ultimate-guide-on-secure-shell-protocol) secure shell is a remarkable protocol that has been used for over twenty-seven years to facilitate seamless communication between remote computers. Now that you have a better understanding of SSH, you can leverage it in your projects to develop unique and secure applications. Good Luck!
    
    **[`^        back to top        ^`](#)**

## `License`
MIT License & [cc](https://creativecommons.org/licenses/by/4.0/) license

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

To the extent possible under law, [Paul Veillard](https://github.com/paulveillard/) has waived all copyright and related or neighboring rights to this work.
