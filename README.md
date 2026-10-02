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


## STEP 6 — Customize the Layout

Go to:

##### Edit → Preferences → Appearance → Layout

Choose a layout where you can clearly see:

- Packet List
- Packet Details
- Packet Bytes or diagram

Click:

Apply → OK

### Description:

A customized layout makes packet investigation easier by keeping the important packet information visible.

<img width="998" height="674" alt="image" src="https://github.com/user-attachments/assets/72e20a7b-fcaa-42b2-bdf2-5bb7e1c9ce5f" />

<img width="997" height="667" alt="image" src="https://github.com/user-attachments/assets/f38d6d37-b8db-4ba4-a8dc-57d72cda9bbf" />


## STEP 7 — Configure Custom Packet Colors

Go to:

#### View → Coloring Rules

Wireshark already provides several default coloring rules.

Click + to create your own.

For example:

### TCP
tcp

### UDP
udp

### DNS
dns

### HTTP
http

### ICMP
icmp

Choose a different background/text color for each rule.

### Description:

Custom colors make different protocols easier to recognize during packet analysis.


<img width="998" height="661" alt="image" src="https://github.com/user-attachments/assets/b5263ddf-a23f-44cb-8ce0-d070f5d7be3b" />

<img width="1004" height="663" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/e3c80d72-45df-4b40-97b5-2e4644029eb9" />

<img width="992" height="663" alt="image" src="https://github.com/user-attachments/assets/0c414346-8707-4128-8d09-6680cd1f8d28" />


## STEP 8 — Create a Packet Capture

Start capturing on your active interface.

While Wireshark is capturing, generate normal traffic from your own Windows computer.

Open Command Prompt.

Run:

ping 8.8.8.8

Let it run for approximately 10 seconds.

Press:

Ctrl + C

### Description:

The ping command generates ICMP Echo Request and Echo Reply packets that can be analyzed in Wireshark.

<img width="980" height="515" alt="Screenshot 2026-10-02 184818" src="https://github.com/user-attachments/assets/72ec9f4b-8c58-49fb-b05a-f3e49cb4dcf0" />

<img width="994" height="663" alt="image" src="https://github.com/user-attachments/assets/7373b633-785a-45bd-9e70-77f71858f4e6" />


## STEP 9 — Generate DNS Traffic

Open Command Prompt and run:

nslookup example.com

You can also open a few normal websites in your browser.

### Description:

DNS traffic shows how your computer requests the IP address associated with a domain name.

<img width="981" height="515" alt="image" src="https://github.com/user-attachments/assets/66073a02-1a4c-400c-80a6-7332ca59758e" />

<img width="1000" height="662" alt="image" src="https://github.com/user-attachments/assets/2464391e-a544-4f0b-98b5-c9a3670f7f94" />


## STEP 10 — Stop the Capture

Return to Wireshark and click the red Stop button.

### Description:

Stopping the capture allows you to analyze the packets collected during the test.

<img width="999" height="663" alt="Screenshot (5)" src="https://github.com/user-attachments/assets/5d0c88a0-1a4a-47b9-a4f1-ada051bb09ac" />


## STEP 11 — Save the Capture

Go to:

File → Save As

Create:

captures

Save the file as:

normal_traffic.pcapng

### Description:

The .pcapng file contains the captured packets and can be reopened later for analysis.

<img width="912" height="710" alt="image" src="https://github.com/user-attachments/assets/3e8526d0-fd87-4e7d-b767-fbe76432e9ab" />
