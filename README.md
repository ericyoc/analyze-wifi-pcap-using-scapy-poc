# Wi-Fi 802.11 Analysis with Scapy

This project demonstrates how to analyze Wi-Fi 802.11 network traffic using Scapy, a powerful Python library for packet manipulation and analysis. The script reads a Wireshark pcap file, performs various filtering and parsing operations, and provides detailed output and a summary table of the findings.

## Wi-Fi 802.11 Frame Format

The 802.11 frame format consists of several fields that provide important information about the wireless communication. The basic structure of an 802.11 frame includes:

- Frame Control: Contains information about the frame type, subtype, and flags.
- Duration/ID: Indicates the duration of the frame or the association ID.
- Address Fields: Includes the source, destination, and BSSID (Basic Service Set Identifier) addresses.
- Sequence Control: Used for fragment numbering and duplicate frame detection.
- Frame Body: Contains the actual data payload of the frame.
- Frame Check Sequence (FCS): Used for error detection.

Understanding the frame format is crucial for analyzing and interpreting the captured network traffic.

## Hacker's Perspective

From a hacker's perspective, analyzing Wi-Fi 802.11 frames can provide valuable information for potential attacks or exploits. Some ways a hacker might use this information include:

- Identifying network SSIDs and BSSIDs to target specific networks.
- Detecting weak or unencrypted networks by analyzing beacon frames and authentication processes.
- Exploiting vulnerabilities in the frame structure or specific frame types.
- Launching denial-of-service attacks by flooding the network with malformed or crafted frames.
- Conducting man-in-the-middle attacks by manipulating or injecting frames.
- Analyzing management frames to gather intelligence about the network infrastructure and connected devices.

It is crucial to understand the potential risks associated with Wi-Fi networks and implement appropriate security measures to protect against malicious activities.

## Summary of Findings

The script generates a summary table that presents the key findings of the pcap analysis. Here's an example of the summary table in GitHub Markdown format:

| Finding                                             | Count/Value   |
|-----------------------------------------------------|---------------|
| TCP Packets                                         | 100           |
| UDP Packets                                         | 50            |
| ICMP Packets                                        | 20            |
| Other Packets                                       | 30            |
| Packets from Source IP 192.168.0.1                  | 75            |
| Packets to Destination Port 80                      | 60            |
| Packets from/to MAC 00:11:22:33:44:55               | 40            |
| Packets in IP Range 192.168.0.1 - 192.168.0.100     | 90            |
| HTTP Packets                                        | 80            |
| Suspicious Packets (Payload > 1024)                 | 10            |
| SYN Packets                                         | 15            |
| Beacon Frame Channels                               | 1, 6, 11      |
| Management Frame: Association Request               |               |
| Management Frame: Association Response              |               |
| Management Frame: Reassociation Request             |               |
| Management Frame: Reassociation Response            |               |
| Management Frame: Probe Request                     |               |
| Management Frame: Probe Response                    |               |
| Management Frame: Beacon                            |               |
| Management Frame: ATIM                              |               |
| Management Frame: Disassociation                    |               |
| Management Frame: Authentication                    |               |
| Management Frame: Deauthentication                  |               |
| Management Frame: Action                            |               |
| DNS Domains                                         | example.com   |
|                                                     | example.net   |
|                                                     | example.org   |

This summary table provides a concise overview of the packet counts, specific filters, management frame types, beacon frame channels, and DNS domains found in the pcap file.

## Conclusion

Analyzing Wi-Fi 802.11 network traffic using Scapy and Wireshark is a powerful technique for understanding network behavior, identifying potential issues, and detecting cybersecurity threats. By leveraging the capabilities of Scapy and the rich information captured in pcap files, network administrators and security professionals can gain valuable insights into wireless network operations and take appropriate actions to ensure the security and integrity of their networks.

It is important to be aware of the potential risks associated with Wi-Fi networks and understand how attackers might exploit vulnerabilities. By analyzing the frame structure, management frames, and other network characteristics, security professionals can develop effective strategies to detect and mitigate potential threats.

Feel free to customize and enhance the script based on your specific analysis requirements and adapt it to your network environment.
