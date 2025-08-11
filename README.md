Task 5 – Network Traffic Capture and Protocol Analysis with Wireshark
1. Objective
Capture and analyze live network traffic using Wireshark, identify at least three different network protocols, and document your findings with explanations and screenshots.

2. Tools & Environment
Operating System: e.g., Windows 11, Kali Linux

Tool Used: Wireshark

3. Steps Performed
3.1 Start a Packet Capture
Opened Wireshark and started a capture session on the main network interface.

![Wireshark Live Capture](Screenshot-2025-08-11-210002.jpg Network Traffic

Generated traffic by pinging websites (e.g., ping google.com), browsing, or using network utilities.

![Kali Ping Session](Screenshot-2025-08-11-205737.jpg Filtering

Used Wireshark's filter bar to isolate traffic for specific protocols (e.g., udp, dns, icmp).

4. Protocols Observed
Protocol	What It Does	Example from Capture
DNS	Resolves hostnames to IP addresses	Queries for google.com (UDP port 53)
ICMP	Tests connectivity (Ping)	Echo requests/replies (e.g., to 142.251.221.238)
UDP	Connectionless transport protocol	DNS, SSDP, NTP, and LAN sync traffic
Example protocol-specific screenshots
DNS Traffic:

![DNS Packets](Screenshot-2025-08-11-205944.jpg:**

![ICMP Ping Packets](Screenshot-2025-08-11-210121.jpg Protocol Descriptions

DNS (Domain Name System):
Converts readable domain names (like google.com) into IP addresses. Captured as queries and responses over UDP port 53.

ICMP (Internet Control Message Protocol):
Used for network diagnostics such as ping. Echo request and reply packets confirm connectivity.

UDP (User Datagram Protocol):
Provides fast, connectionless packet delivery. Used for applications like DNS, LAN discovery, and time sync (NTP).

6. What I Learned (Reflection)
Wireshark provides clear visualization and analysis of real network traffic.

Protocol filtering techniques quickly reveal patterns and issues across DNS, ICMP, UDP, etc.

Understanding these protocols is foundational for troubleshooting and cybersecurity.

7. Appendix
Screenshots: Included above in each section for clarity.

Packet Capture File: (Optional) Attach your .pcap file if needed for review.

Wireshark Tips:

To filter by DNS: enter dns in the filter bar.

For ICMP: icmp

For UDP: udp

