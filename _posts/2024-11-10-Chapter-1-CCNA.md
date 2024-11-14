---
title: Chapter 1 Notes
date: 2024-11-10 12:00:00 -500
categories: [CCNA]
tags: [ccna,learning]
---


#### Exam Topics Covered

1.0 Network Fundamentals
- 1.3 Compare interface and cabling types
- 1.3.a Single-mode fiber, multimode fiber and copper
- 1.3.b Connections (Ethernet shared media and point-to-point)

---
### Key terms


*Segment*
*Ethernet Frame*
*Encapsulation*
*De-encapsulation*


---

## Notes

In networking diagrams the cloud normally represents details not important to the diagram 
## History Leading up to TCP/IP
- Network models began as vendor specific
- International Organization for Standardization came out with the OSI Model
- DOD contracted research developed TCP/IP
- In the 1990's both OSI model and TCP/IP model where in use
- By end of the 1990's OSI fell to wayside with TCP/IP dominating
### Overview of TCP/IP Model
- TCP/IP Refrences and defines a large collection of protocols that allow devices to communicate
- Protocols are defined as RFC (Request for Comments)
- TCP/IP avoids repeated work by simply referring to standards/protocols provided by 3rd party
	- Ex. ethernet is defined by as RFC but refers to IEEE ethernet as an option

| TCP/IP model Layers                                                      |
| ------------------------------------------------------------------------ |
| Application                                                              |
| Transport                                                                |
| Network AKA IP Layer - Responsible for delivering data across whole path |
| Datalink - focuses on rules that control use of physical link            |
| Physical - Focuses how to transmit data over link                        |
- Different computer components implement different protocols/standards
- Example layers and Protocols
	- Application - HTTPS,POP3,SMTP
	- Transport - TCP/UDP
	- Network - IP,ICMP
	- Datalink - Ethernet, 802.11
### TCP/IP Application Layer
- App layer does not define application, Defines services that the application needs
	- Provides interface between software running on computer and network itself
	- Web Browser is an example
#### HTTP Overview
- Hypertext Transfer Protocol
- Developed 1990s
- URL - Uniform Resource Locators
- URI - Uniform Resource Identifier
- Protocols generally use headers to put info used by that protocol
	- 200 - OK
	- 404 - Not Found
### TCP/IP Transport Layer
- 2 most common used protocols
	- TCP - Transmission Control protocol
		- Error recovery based
		- Each layer Provides service to layer above it
		- To recover from errors TCP uses concept of Acknowledgements
	- UDP - User Datagram Protocol
#### Same Layer & Adjacent Layer
Adjacent layer interaction - how adjacent layers on same computer work together
Same layer interaction - when 2 computers want to communicate on the same layer 
### TCP/IP Network Layer
- Network layer hold small number of protocols
- Only one  major protocol
	- IP (Internet Protocol)
		- Used for features such as addressing and routing
#### IP Addressing Basics
Dotted Decimal notion 0.0.0.0
### TCP/IP Data Link and Physical Layer
- Defines protocols and hardware required to deliver data across some physical network
- Some protocols define both Datalink and Physical Layer functions
- Physical Layer defines cabling as well as how energy passes through it
- Sending IP Packets the host/router uses link layer details to send packet on
#### Ethernet Frame
- Made up of:
	- Ethernet Header
	- IP Packet
	- Ethernet Trailer
- Frame
	- IP Packet with Ethernet Header and Trailer
- De-encapsulate 
	- At this level it is the removal of the Ethernet Header/Trailer leaving IP Packet