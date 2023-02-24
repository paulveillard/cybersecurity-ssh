# SSH (Secure Socket Shell)

An ongoing & curated collection of awesome software best practices and techniques, libraries and frameworks, E-books and videos, websites, blog posts, links to github Repositories, technical guidelines and important resources about Secure Socket Shell (SSH) in Cybersecurity.
> Thanks to all contributors, you're awesome and wouldn't be possible without you! Our goal is to build a categorized community-driven collection of very well-known resources.

## `Table of Contents`
- [About SSH]()
- [What is SSH Exactly?]()
- [How Does SSH work]()
- [SSH Server]()
- [SSH Client]()
- [Encryption Key]()
- [What is SSH Typically used for?]()
- [Is SSH Vulnerable]()
- [Inadequate SSH Key sharing]()
- [Frequent Sharing of SSH Keys]()
- [Static SSH keys and embedded keys]()
- [Further Reading]()


### `About SSH? A Beginner's guide to Secure SSH`

![Secure Socket Shell](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/secure-shell-protocol.jpg)
- A Secure Shell, or Secure Socket Shell, [SSH](https://en.wikipedia.org/wiki/Secure_Shell) is a network protocol that allows devices to achieve two important things: communicate and share data. Additionally, the SSH protocol also encrypts data, making it ideal for unsecured networks.

### `What is SSH Exactly?`


As a term, Secure Socket Shell, defines both a cryptographic network protocol and the programs that enable it to work.

> SSH enables network administrators to access a computer via an unsecured network in a safe manner. It ensures a secure connection that allows it to operate and manage remote computers without worrying about the safety of shared data.  

To achieve this, the SSH protocol does not only provide encryption with the help of a secure channel but also strong password authentication and public-key authentication.

![ssh-1.0](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-1.0.png)

The SSH protocol and SSH keys – access credentials within the protocol – secure millions of file transfers, automated functions and upkeep sessions per day. 

Continue reading if you wish to learn more about SSH servers and the client programs that enable reaching them. As well as the primary use cases of the SSH protocol and its vulnerabilities.


### `How does SSH work?`



> SSH uses the client-server model to connect the application and the server, or the location where the session is shown and the place where it’s actually running.
![ssh-2](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-1.png)

> In other words, the SSH clients contact SSH servers to begin the connection setup process. An SSH server sends its public key, and with the help of public-key cryptography, the client tries to verify the server’s identity. 

Once this is over, the SSH protocol starts using strong symmetric encryption protocols and hashing algorithms to establish privacy and secure file transfers. This is how data is exchanged between client and server safely.

SSH client and server do this with the help of various encryption methods, but the most common ones are Blowfish and the Advanced Encryption Standard. 

Blowfish is the oldest symmetric encryption algorithm. However, the Advanced Encryption Standard, developed by the National Institute of Standards and Technology, is used more widely. 



SSH also works similarly to a typical Virtual Private Network (VPN). A VPN also creates an encrypted tunnel for secure communication. The only difference is that a VPN doesn’t use the client-server model but, instead, a secure connection between your device and the VPN server.

It is also important to note that the SSH secure connection works differently on different operating systems:

    On Mac and Linux – via Terminal
    On Windows – via an installed SSH client 

The client-server relationship can be tricky to understand. So, let’s delve into how both SSH servers and SSH clients work. 



### `SSH Server`



As stated previously, the SSH server is always the one that initiates the network connection. However, it also stays vigilant for new connections and responds to them. The server does that using the host system’s TCP port 22. 



At the start of every SSH connection, the server must authenticate itself to the client using public-key cryptography. This client authentication is necessary so the SSH client can make sure it’s communicating with a legitimate server and not an attacker.

Once the client and the server establish a safe connection, users can perform:

    File transfers
    Remote command execution
    Remote host administration
    Other application traffic security
    
 ![ssh-4](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-3.png)

- Unfortunately, the SSH server is often the chosen target of cyberattackers as it provides remote access to the host system. Due to that, the software quality must be high, and the server must have strict security requirements. In other words, its code has to be reliable to prevent bugs and imperfections that could lead to unnecessary exposure. 


### `SSH Client`

System administrators can benefit from secure connections by installing a program on their local machine and the remote computer. This software is known as the Secure Socket Client. There are many popular SSH client services on the web to choose from for local and remote computers. 

While Mac and Linux devices typically use a Terminal program, the Windows operating system requires a dedicated client program to run SSH commands. For example, PuTTY, KiTTY, MobaXterm or WinSCP. 

Once you have a client installed on a local machine, you also have to install an SSH server to accept SSH connections. This is how you can start using this secure alternative to regular remote access options. Essentially, the client acts as a secure environment, via which you connect to a remote host device.

When it comes to SSH authentication, you use a username and password. You can also use a public-private key pair for secure remote access management without a password. 


### `Encryption key`

The encryption key is a form of user authentication within the SSH protocol. 

> SSH keys are a secure alternative compared to regular passwords, and they enable secure automation. For example, automated file transfers. They are often used in configuration management tools, scripts and backup systems, too.

> SSH keys are, effectively, a cryptographic key pair that comprises a private key and a public key.

The public key is configured on the server in a unique public key file format. To permit access to a user with a copy of the corresponding private key. And thanks to this unique public-to-private-key relationship, encrypted keys are much safer than passwords. 

However, the system is not perfect, which is why you should also use a passphrase, as it encrypts the private key. 

The passphrase can protect against key leaking and ensure that a cyberattacker cannot complete a successful public key authentication. In short, hackers can gain access to private keys, but they are useless if they are encrypted with a passphrase. 

Unfortunately, it is estimated that more than 90% of SSH keys in large corporations don’t have a passphrase. Undoubtedly, that is a considerable security risk. 

- The good news is that you can deal with this by implementing various SSH key management practices that can help create a more secure network. 


### `What is SSH typically used for?`



The SSH protocol is most notably used in data centers where it provides:

    Remote access to various resources
    Secure management
    The delivery of software patches
    Virtualization platform administration
    Secure router management
    Server hardware maintenance

![ssh-42](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-4.png)

In almost all data centers, SSH comes together with Mac, Unix and Linux operating systems.  

The SSH network protocol is ideal for network administrators looking to gain secure remote login access to remote systems. They routinely use the protocol to execute commands for testing applications, rebooting systems, automating data transfers and so much more. 

- SSH is highly useful for major companies as well. Corporations use the SSH protocol to complete encrypted file transfers and thus avoid other less secure file transfer methods. The Internet Engineering Task Force (IETF) created the SSH File Transfer Protocol (SFTP) as an extension to SSH to ensure that every file transfer is secure.



Corporations also use the protocol to complete various automated tasks like:

    Reporting
    System backup
    Data backup
    Data archiving
    Database cleanups
    Network maintenance

Smaller businesses can also benefit from employing the SSH protocol. For example, they can use it to share files with their customers in a secure way. 

Overall, SSH is beneficial for establishing encrypted connections, no matter the actual use case. SSH traffic is always encrypted. Therefore, a Te looking to protect their privacy while browsing or transferring files can benefit from the Secure Shell protocol. 


### `Is SSH vulnerable?`
![ssh-5](https://github.com/paulveillard/cybersecurity-ssh/blob/main/img/ssh-5.png)

SSH communications security is not perfect. Thankfully, we know its flaws, and they typically stem from SSH keys and their improper use. 

For example, we know that SSH keys can be stolen, and hackers can then use them as a backdoor to vulnerable systems. This is not uncommon, and it is usually linked to people focusing on protecting their credentials only, forgetting entirely about the protection of the keys.

The problem here is that when an attacker gains access to an SSH key, they also gain access to all other keys stored on the device. Basically, if they can get their hands on only a couple of the keys, they might be able to gain remote user access to the entire company. 



Let’s take a look at a couple of SSH vulnerabilities that you should be particularly cautious about:

    Inadequate SSH key tracking
    Frequent sharing of SSH keys
    Static SSH keys and embedded keys



### `Inadequate SSH key tracking`

Large companies usually accumulate a massive number of SSH keys. If they have 10,000 or more servers, they have millions of keys. Therefore, it’s no wonder they might lose track of some of them. 

However, this can easily lead to hackers gaining access to the unaccounted keys. As a result, they may gain long-term access to the company. 


### `Frequent sharing of SSH keys`

Unfortunately, some employees duplicate keys thinking that they could use them more efficiently. 

That said, an attacker only needs a couple of keys to gain unauthorized access. This is why SSH key sharing is something that should be monitored closely and limited when possible.


### `Static SSH keys and embedded keys`

Security professionals and IT administrators don’t often change keys because they fear that something might be forgotten along the way. However, this creates a lot of static keys, which can quickly open a backdoor for potential cyberattackers, should they find them. 

Furthermore, keys embedded within scripts and applications can also become static. Administrators avoid changing them as they don’t understand the underlying code and they don’t want to cause a system outage. But these static embedded keys can become an issue just like other static SSH keys. 


### `Further Reading`

[SSH](https://www.ipxo.com/blog/what-is-ssh/) might be one of the more complicated network protocols. However, the reason for its wide use and popularity is simple: All communication between the SSH client and server is entirely encrypted and, therefore, incredibly safe. 

Naturally, the [SSH] protocol is not without its faults. That said, it is still much better than other authentication methods. It can prove very beneficial to practically any business that needs a secure method of sharing files and communicating over the internet.

If you are looking to start using SSH, we hope that this guide has helped you understand how it works, what it is used for and how you can use it safely.


**[`^        back to top        ^`](#)**

## `License`
MIT License & [cc](https://creativecommons.org/licenses/by/4.0/) license

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

To the extent possible under law, [Paul Veillard](https://github.com/paulveillard/) has waived all copyright and related or neighboring rights to this work.
