# **Cybersecurity Incident Report \- Network Attack**

| Section 1: Identify the type of attack that may have caused this  network interruption |
| :---- |
| **One potential explanation for the website's connection timeout error message is:** The system is being overloaded and is a victim of a DoS attack.  **The logs show that:** The server is struggling to respond because of too many SYN packet requests coming from an unfamiliar IP address.  **This event could be:** A type of DoS attack known as a SYN flood attack.  |
|  |

| Section 2: Explain how the attack is causing the website to malfunction |
| :---- |
| **When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake:** The client/source sends a SYN packet to the server/destination.  The server responds to the request with a SYN-ACK signal and accepts the connection. (Some resources are reserved by the destination to connect.)  The client then sends an ACK packet acknowledging the request and a reliable connection is formed.  **Explain what happens when a malicious actor sends a large number of SYN packets all at once:** The malicious actor sends a large amount of SYN packets simultaneously and the server is overwhelmed by the excessive volume of requests/incoming traffic and loses its ability to respond/function. (There are no available server resources left for any legitimate TCP connection requests.)  **Explain what the logs indicate and how that affects the server:** There are a suspicious amount of TCP SYN requests all coming from an unfamiliar IP address which is preventing the server from responding to legitimate server requests causing a connection timeout error for clients.  |

