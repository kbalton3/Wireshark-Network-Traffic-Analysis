# Wireshark Network Traffic Analysis

## Project Overview

This project demonstrates hands-on network traffic analysis using Wireshark. I captured and analyzed network traffic from my local system to better understand how common network protocols operate and how packet analysis can be used for troubleshooting.

The analysis focused on DNS resolution, TCP connection establishment, TLS/HTTPS communication, and ICMP connectivity testing.

## Objectives

- Capture live network traffic using Wireshark
- Analyze DNS queries and responses
- Examine the TCP three-way handshake
- Identify TLS/HTTPS traffic
- Analyze ICMP Echo Request and Echo Reply packets
- Use Wireshark display filters to isolate specific network protocols
- Practice interpreting packet headers, IP addresses, ports, and protocol behavior

## Lab Environment

- macOS
- Wireshark
- Terminal
- Wi-Fi network interface (en0)

## DNS Analysis

DNS traffic was filtered and analyzed to observe the name-resolution process. A DNS query for `example.com` was sent from the local system to the DNS server, followed by a successful response containing IPv4 addresses associated with the domain.

This demonstrated how DNS translates human-readable domain names into IP addresses that systems can use for network communication.

## TCP Three-Way Handshake

TCP traffic was analyzed to identify the connection establishment process.

The capture demonstrated the three stages of the TCP handshake:

1. SYN
2. SYN-ACK
3. ACK

The analysis showed the local system establishing a connection with a remote server over TCP port 443, which is commonly used for HTTPS communication.

## TLS/HTTPS Analysis

After the TCP connection was established, TLS traffic was examined. The capture included a TLS Client Hello message and subsequent encrypted application traffic.

The analysis demonstrated how TLS is used to establish secure communication before encrypted application data is exchanged between a client and server.

## ICMP Connectivity Analysis

ICMP traffic was generated using the `ping` command against `8.8.8.8`.

Four ICMP Echo Requests were transmitted and four corresponding Echo Replies were received, resulting in 0% packet loss.

Wireshark was used to verify the request and reply packets and inspect ICMP fields including packet type, sequence number, source address, and destination address.

## Key Findings

The packet capture demonstrated the sequence of network communications involved in common network activity:

**DNS Resolution → TCP Connection → TLS/HTTPS Communication**

ICMP analysis was also used to verify basic IP connectivity and observe request/reply behavior.

## Skills Demonstrated

- Wireshark packet capture
- Packet analysis
- Network troubleshooting
- DNS analysis
- TCP/IP fundamentals
- TCP three-way handshake analysis
- TLS/HTTPS traffic analysis
- ICMP analysis
- Wireshark display filters
- Network protocol interpretation

## Security Note

The original packet capture is stored locally and is not included in this public repository because packet capture files may contain network metadata or unrelated traffic.
