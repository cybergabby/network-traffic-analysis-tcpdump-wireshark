# Network Traffic Analysis Lab (TCPDump + Wireshark)

## 📌 Overview
This project demonstrates how network traffic flows across a system and how to analyze it using TCPDump and Wireshark.


<img width="1014" height="736" alt="wireshark2" src="https://github.com/user-attachments/assets/4ec5e548-0bd5-47cc-82bd-57b2e4750ba8" />
<img width="1366" height="724" alt="wireshark 4" src="https://github.com/user-attachments/assets/1ae99753-51dc-4bca-b383-d6d6964d4bcd" />
<img width="1366" height="537" alt="wireshark1" src="https://github.com/user-attachments/assets/227f91fd-988b-4b24-abb8-b9a029b2969c" />

The goal is to understand packet-level communication, identify protocols, and detect basic network behaviors.


## 🛠️ Tools Used
- TCPDump (packet capture)
- Wireshark (packet analysis)


## 🌐 Network Activity Simulated
- ICMP (Ping)
- DNS Queries
- ARP Requests
- Basic Network Communication


## Traffic Analysis

### 1. ICMP (Ping Traffic)

<img width="1366" height="620" alt="wireshark 5" src="https://github.com/user-attachments/assets/04b3cc61-ca79-469d-aeb8-d4f636d3ef01" />


- Echo request and reply observed
- Sequence numbers track packet flow
- TTL values indicate hop count

📌 Insight:
Used to test connectivity. Abnormal spikes may indicate ICMP flood attacks.


### 2. DNS Traffic

<img width="1366" height="738" alt="DNSwireshark 3" src="https://github.com/user-attachments/assets/df9f2477-d417-4fed-9b1b-61f70df42aa5" />


- Domain resolution for `google.com`
- A and AAAA records observed
- PTR records used for reverse lookup

📌 Insight:
DNS traffic reveals user activity and can expose malicious domains.


### 3. ARP Traffic

<img width="1366" height="768" alt="wireshark Arp" src="https://github.com/user-attachments/assets/10c43ba7-687d-4793-b0da-4c366671fc29" />


- IP-to-MAC resolution observed

📌 Insight:
Frequent ARP traffic can indicate scanning or spoofing attempts.

### 4. Packet Structure Breakdown

Each packet follows TCP/IP encapsulation:

- Application → DNS
- Transport → UDP
- Internet → IP
- Network → Ethernet


## Key Learnings

- Understood how data is encapsulated across layers
- Identified real network protocols in live traffic
- Analyzed packet structure using Wireshark
- Observed normal vs potential suspicious patterns


## 📎 Author
Gabriel Odusanya
