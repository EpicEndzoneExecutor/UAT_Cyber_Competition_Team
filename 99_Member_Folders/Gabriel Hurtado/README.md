Intro to Offensive Security 

Offensive security is the process of breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access to them. 
 
My first hack 
 
Step 1 Open a terminal 

A terminal or something called the command-line, allows us to interact with a computer without using a graphical user interface GUI 

 

 
Step 2 Find the hidden Website Pages 
 
Most companies will have an admin portal page, giving their staff access to basic admin controls for day-to-day operations. For a bank, an employee might need to transfer money to and from client accounts. Often these pages are not made private, allowing attackers to find hidden pages that show, or give access to, admin controls or sensitive data.  
 
 
Type the following command into the terminal to find potentially hidden pages 

 

gobuster -u http://fakebank.com -w wordlist.txt dir 
 
In the command above, -u is used to state the website we're scanning, -w takes a list of words to iterate through to find hidden pages. 

You should have found a secret bank transfer page that allows you to transfer money between accounts at the bank (/bank-transfer). Type the hidden page into the FakeBank website on the machine. Good Job Free bands now. 

 

Introduction to Defensive Security 
 

Defensive security is somewhat the opposite of offensive security, as it is concerned with two main tasks: 

 

    Preventing intrusions from occurring 

    Detecting intrusions when they occur and responding properly 

 

 

Some of the tasks that are related to defensive security include: 

User cyber security awareness  

Documenting and managing assets 

Updating and patching systems 

Setting up preventative security devices 

Setting up logging and monitoring devices 

 

(SOC) 

A Security Operations Center (SOC) is a team of cyber security professionals that monitors the network and its systems to detect malicious cyber security events. 

 

Threat Intelligence 

 

Refers to information you gather about actual and potential enemies. A threat is any action that can disrupt or adversely affect a system. Threat intelligence aims to gather information to help the company better prepare against potential adversaries. The purpose would be to achieve a threat-informed defense. 

 

Digital Forensics 

 

Forensics is the application of science to investigate crimes and establish facts. With the use and spread of digital systems, such as computers and smartphones, a new branch of forensics was born to investigate related crimes: computer forensics, which later evolved into, digital forensics. 

 

Incident Response 

 

An incident usually refers to a data breach or cyber attack; however, in some cases, it can be something less critical, such as a misconfiguration, an intrusion attempt, or a policy violation. Examples of a cyber attack include an attacker making our network or systems inaccessible, defacing (changing) the public website, and data breach (stealing company data). How would you respond to a cyber attack? Incident response specifies the methodology that should be followed to handle such a case. The aim is to reduce damage and recover in the shortest time possible. 

 

Malware Analysis 

Malware stands for malicious software. Software refers to programs, documents, and files that you can save on a disk or send over the network. 

 

Virus is a piece of code that attaches itself to a program. It is designed to spread from one computer to another; moreover, it works by altering, overwriting, and deleting files once it infects a computer. The result ranges from the computer becoming slow to unusable. 

Trojan Horse is a program that shows one desirable function but hides a malicious function underneath. For example, a victim might download a video player from a shady website that gives the attacker complete control over their system. 

Ransomware is a malicious program that encrypts the user’s files. Encryption makes the files unreadable without knowing the encryption password. The attacker offers the user the encryption password if the user is willing to pay a ransom. 

 

 

What is Networking? 

 

 In computing, a network can be formed by anywhere from 2 devices to billions. These devices include everything from your laptop and phone to security cameras, traffic lights and even farming! 

 

The Internet is one giant network that consists of many, many small networks within itself. 

 

The first iteration of the Internet was within the ARPANET project in the late 1960s. This project was funded by the United States Defence Department and was the first documented network in action. However, it wasn't until 1989 when the Internet as we know it was invented by Tim Berners-Lee by the creation of the World Wide Web (WWW). It wasn't until this point that the Internet started to be used as a repository for storing and sharing information, just like it is today. 

 

IP Addresses 

 

An IP address (or Internet Protocol) address can be used as a way of identifying a host on a network for a period of time, where that IP address can then be associated with another device without the IP address changing. 

 

An IP address is a set of numbers that are divided into four octets. The value of each octet will summarise to be the IP address of the device on the network. This number is calculated through a technique known as IP addressing & subnetting, but that is for another day. What's important to understand here is that IP addresses can change from device to device but cannot be active simultaneously more than once within the same network. 

 

IPv6 is a new iteration of the Internet Protocol addressing scheme to help tackle this issue. Although it is seemingly more daunting, it boasts a few benefits: 

Supports up to 2^128 of IP addresses (340 trillion-plus), resolving the issues faced with IPv4 

More efficient due to new methodologies 

 

Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard. This network interface is assigned a unique address at the factory it was built at, called a MAC (Media Access Control ) address. The MAC address is a twelve-character hexadecimal number (a base sixteen numbering system used in computing to represent numbers) split into two's and separated by a colon. These colons are considered separators. For example, a4:c3:f0:85:ac:2d. The first six characters represent the company that made the network interface, and the last six is a unique number. 

 

OSI model 

 

The Open Systems Interconnection model is a reference model from the International Organization for Standardization that "provides a common basis for the coordination of standards development for the purpose of systems interconnection." In the OSI reference model, the communications between systems are split into seven different abstraction layers: Physical, Data Link, Network, Transport, Session, Presentation, and Application. The model partitions the flow of data in a communication system into seven abstraction layers to describe networked communication from the physical implementation of transmitting bits across a communications medium to the highest-level representation of data of a distributed application. Each intermediate layer serves a class of functionality to the layer above it and is served by the layer below it. Classes of functionality are realized in all software development through all standardized communication protocols. 

 

Packets and Frames  

 

Packets and Frames are the names given to Protocol data units (PDUs) at different network layers  

 

Segments are units of data in the Transport Layer (TCP/UDP in case of the Internet)  

Packets are units of data in the Network Layer (IP in case of the Internet)  

Frames are units of data in the Link Layer (e.g. Wifi, Bluetooth, Ethernet, etc). 

Port Forwarding 

 

In computer networking, port forwarding or port mapping is an application of network address translation that redirects a communication request from one address and port number combination to another while the packets are traversing a network gateway, such as a router or firewall. This technique is most commonly used to make services on a host residing on a protected or masqueraded network available to hosts on the opposite side of the gateway, by remapping the destination IP address and port number of the communication to an internal host. 

 

Firewalls 

A firewall is a network security device that monitors incoming and outgoing network traffic and decides whether to allow or block specific traffic based on a defined set of security rules. 

Firewalls have been a first line of defense in network security. They establish a barrier between secured and controlled internal networks that can be trusted and untrusted outside networks, such as the Internet.  

A firewall can be hardware, software, software-as-a service (SaaS), public cloud, or private cloud (virtual). 

A stateful firewall inspects everything inside data packets, the characteristics of the data, and its channels of communication. Examines the behavior of data packets, and if anything seems off, they can filter out the suspicious data. 
 
Stateless firewalls make use of a data packet's source, destination, and other parameters to figure out whether the data presents a threat. 

 

 

VPN 

 

A Virtual Private Network (or VPN for short) is a technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the Internet (known as a tunnel). Devices connected within this tunnel form their own private network. 

 

 

PPP 

This technology is used by PPTP (explained below) to allow for authentication and provide encryption of data. VPNs work by using a private key and public certificate (similar to SSH). A private key & certificate must match for you to connect. 

This technology is not capable of leaving a network by itself (non-routable). 

 

 

PPTP 
	

 

The Point-to-Point Tunneling Protocol (PPTP) is the technology that allows the data from PPP to travel and leave a network.  

PPTP is very easy to set up and is supported by most devices. It is, however, weakly encrypted in comparison to alternatives. 

 

 

IPSec 

 

Internet Protocol Security (IPsec) encrypts data using the existing Internet Protocol (IP) framework. 

IPSec is difficult to set up in comparison to alternatives; however, if successful, it boasts strong encryption and is also supported on many devices. 

 

LAN Networking Devices 

 

Router 

 
A router is a computer and networking device that forwards data packets between computer networks, including internetworks such as the global Internet. A router is connected to two or more data lines from different IP networks. 

 

 

Switch 

 

A network switch connects devices in a network to each other, enabling them to talk by exchanging data packets. Switches can be hardware devices that manage physical networks or software-based virtual devices. 

 

DNS 

 

The Domain Name System is a hierarchical and distributed name service that provides a naming system for computers, services, and other resources on the Internet or other Internet Protocol networks. It associates various information with domain names assigned to each of the associated entities. 

 

Domain Hierarchy 

 

Top-Level Domain (TLD) 

  

A TLD refers to the rightmost segment of a domain name. For instance, in tryhackme.com, the TLD is .com. There are two primary categories of TLDs: Generic Top-Level Domains (gTLDs) and Country Code Top-Level Domains (ccTLDs). Traditionally, gTLDs indicate the intended use of the domain—.com for commercial, .org for organizations, .edu for education, and .gov for government entities. Conversely, ccTLDs specify geographical locations, such as .ca for Canada, .co.uk for the United Kingdom, etc. Due to increasing demand, numerous new gTLDs have emerged, including .online, .club, .website, and .biz, among others.  

  

Second-Level Domain 

  

In the example of tryhackme.com, "tryhackme" is the Second-Level Domain (SLD). When you register a domain, the SLD can include up to 63 characters plus the TLD and can use letters (a-z), numbers (0-9), and hyphens—though it cannot start or end with a hyphen, nor can it have consecutive hyphens. 

  

Subdomain 

  

A subdomain is positioned to the left of the SLD and separated by a period. For example, in admin.tryhackme.com, "admin" is the subdomain. Subdomains follow the same naming rules as SLDs: they are limited to 63 characters and can only include letters, numbers, and hyphens. Subdomains can be extended with additional levels, such as jupiter.servers.tryhackme.com, but the total length must not exceed 253 characters. There are no limits on the number of subdomains that can be added to a domain. 

 

 

DNS Record Types 

  

DNS serves more than just websites, and there are several types of DNS records you might encounter. 

  

A Record 

 

These records map domain names to IPv4 addresses, such as 104.26.10.229. 

  

AAAA Record 

 

These records map domain names to IPv6 addresses, like 2606:4700:20::681a:be5. 

  

CNAME Record 

 

This type of record points a domain to another domain name. For example, the subdomain store.tryhackme.com might point to shops.shopify.com via a CNAME record. A subsequent DNS query is then made to shops.shopify.com to resolve its IP address. 

  

MX Record 

 

MX records direct to the servers managing email for a domain. For instance, an MX record for tryhackme.com might direct to alt1.aspmx.l.google.com. These records often include a priority setting that indicates the order in which servers should be tried, useful for routing emails to backup servers if the primary one fails. 

  

TXT Record 

 

TXT records are versatile text fields used for various purposes. They can specify which servers are authorized to send emails for a domain, aiding in anti-spam efforts, or confirm domain ownership during registrations with third-party services. 

 

 
