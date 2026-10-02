# Wireshark-Network-Traffic-Analysis-Project


## 1. Introduction

Wireshark is a network packet analyzer used to capture, inspect, and analyze network traffic. This project demonstrates Wireshark installation, configuration, packet capture, display filters, custom coloring, protocol analysis, and basic security analysis.


## 2. What is Wireshark?

Wireshark is an open-source network protocol analyzer that captures network packets and displays detailed information about network communication.It is commonly used by SOC analysts, network administrators, penetration testers, and security professionals for troubleshooting and security monitoring.

### Main uses

- Capture network packets
- Analyze network protocols
- Troubleshoot network problems
- Investigate suspicious traffic
- Identify communication between systems
- Support security investigations


## 3. Project Objectives

By completing this project, you will demonstrate:

- Wireshark installation on Windows
- Network-interface selection
- Custom Wireshark layout
- Custom packet-coloring rules
- Display filters
- TCP/UDP analysis
- DNS analysis
- HTTP/HTTPS analysis
- ICMP analysis
- Packet capture and .pcapng files
- Basic security analysis
- GitHub documentation


## 4. Requirements

- Software
- Windows 10/11
- Wireshark
- Web browser
- Command Prompt


## STEP 1 — Install Wireshark

Download and install Wireshark for Windows from the official site:

[Wireshark official website](https://www.wireshark.org/?utm_source=chatgpt.com)

During installation, make sure Npcap is selected when the installer offers it.

### Description :
Npcap allows Wireshark on Windows to capture packets from network interfaces.

<img width="565" height="432" alt="wrsrk 1" src="https://github.com/user-attachments/assets/5c475e80-66f8-48a0-b2c7-229cc0f0f7f4" /><img width="518" height="401" alt="wrsrk 3" src="https://github.com/user-attachments/assets/32b4763f-0043-46fc-a66f-9a4c8959779c" />


## STEP 2 — Open Wireshark

Open:

Start → Wireshark

You will see available network interfaces such as:

Wi-Fi
Ethernet

You will also see traffic graphs beside active interfaces.

### Description:

The Wireshark home screen shows the network interfaces available for packet capture.
