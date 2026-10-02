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

<img width="565" height="432" alt="wrsrk 1" src="https://github.com/user-attachments/assets/5c475e80-66f8-48a0-b2c7-229cc0f0f7f4" />


## STEP 2 — Open Wireshark

Open:

Start → Wireshark

You will see available network interfaces such as:

- Wi-Fi
- Ethernet

You will also see traffic graphs beside active interfaces.

### Description:

The Wireshark home screen shows the network interfaces available for packet capture.

<img width="1000" height="660" alt="02-wireshark-home" src="https://github.com/user-attachments/assets/d7a2d9a9-a716-49fc-aefa-a01eada772c4" />


## STEP 3 — Identify Your Active Interface

If you are connected through Wi-Fi, select:

Wi-Fi

If you are using a network cable, select:

Ethernet

You can confirm your connection using Windows Command Prompt:

ipconfig

Look for:

IPv4 Address

### Description:

ipconfig helps identify the Windows network adapter and its assigned IP address.

## STEP 4 — Start Packet Capture

In Wireshark, double-click:

Wi-Fi

or:

Ethernet

Packets should start appearing.

### Description:

Wireshark now captures network packets passing through the selected Windows network interface.

<img width="997" height="684" alt="image" src="https://github.com/user-attachments/assets/7f7b4a37-2438-49a5-a6e6-5c461c533d7c" />


## STEP 5 — Understand Wireshark Layout

Wireshark normally contains three main areas:

#### Packet List Pane

Shows captured packets.

#### Packet Details Pane

Shows detailed protocol information for the selected packet.

#### Packet Bytes Pane

Shows the raw packet data in hexadecimal and ASCII.

### Description:

These panes allow you to move from a high-level packet view to detailed protocol information.

<img width="997" height="685" alt="image" src="https://github.com/user-attachments/assets/86d843c6-3e5b-402b-92c1-fb16f01c9506" />
