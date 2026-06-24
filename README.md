# Network Traffic Analysis Using Wireshark
### SOC Investigation Report | Pramodh Prakash

---

## About This Project

This project is a hands-on network traffic analysis exercise 
carried out from a SOC analyst perspective using Wireshark. 
Real network traffic was captured on a live Windows machine 
and analyzed protocol by protocol to understand normal 
behavior and identify potential security threats.

---

## Analyst Profile

| Field | Details |
|-------|---------|
| Name | Pramodh Prakash |
| Education | MSc Cybersecurity, NTU UK |
| Experience | 1 Year - Network Engineer, Cisco |
| Certification | CCNA |

---

## Tools Used

- Wireshark
- Command Prompt (Windows)
- Web Browser

---

## Protocols Analyzed

| Protocol | Filter Used | SOC Relevance |
|----------|-------------|---------------|
| DNS | dns | Malicious domain detection, C2 communication, DNS tunneling |
| ICMP | icmp | Ping sweep detection, ICMP flood, ICMP tunneling |
| TCP | tcp | Port scanning, SYN flood, C2 connections |
| HTTP | http | Credential theft, web shell access, downgrade attacks |
| ARP | arp | ARP spoofing, Man in the Middle attacks |
| UDP | udp | DNS tunneling, UDP flood, QUIC abuse |
| DHCP | dhcp | Rogue DHCP server, DHCP starvation |

---

## Key Findings

- Captured complete DNS resolution flow including CNAME 
  aliases and dual-stack IPv4/IPv6 responses
- Observed Airtel ISP blocking einthusan.tv using 
  Response Policy Zone (RPZ) — real-world DNS filtering
- Captured clean ICMP echo request/reply with TTL 
  analysis showing 11 network hops to Google
- Observed TCP connections on port 443 with TLS 
  encryption and graceful FIN ACK termination
- Captured HTTP 301 redirect from HTTP to HTTPS — 
  real-world security redirect in action
- Observed complete ARP request/reply exchange showing 
  MAC address resolution in under 1 millisecond
- Captured QUIC protocol traffic over UDP showing 
  Google's modern encrypted transport in action
- Observed DHCP Request/ACK showing IP address 
  reconfirmation without full DORA handshake

---

## Files in This Repository

| File | Description |
|------|-------------|
| Wireshark_SOC_Report_Pramodh.docx |  Full SOC investigation report with screenshots |

---

## Resume Line

Performed network traffic analysis using Wireshark by 
capturing and analyzing DNS, ICMP, TCP, TLS, ARP, HTTP, 
UDP and DHCP traffic from a SOC investigation perspective. 
Documented findings in a structured SOC report format 
with protocol-level analysis and threat detection use cases.

---

## Connect

LinkedIn: www.linkedin.com/in/pramodh-prakash
