# Enterprise Split-Firewall Network

> A secure enterprise network architecture featuring split-firewall design, site-to-site IPsec VPN connectivity, NAT, static routing, and layered security controls. This project simulates communication between headquarters and a remote branch while enforcing secure traffic flow across multiple network security zones.

---

## Overview

This project implements a dual-site enterprise network that connects a Headquarters (HQ) and a Remote Branch through an IPsec VPN tunnel over the public Internet.

Each site follows a **split-firewall architecture**, where perimeter and internal firewalls separate Internet traffic, DMZ resources, VPN gateways, and internal networks. The design demonstrates layered network defense, secure routing, network address translation (NAT), and firewall policy enforcement.

---

## Project Objectives

- Design a multi-site enterprise network
- Implement layered firewall security
- Configure static routing
- Configure NAT and PAT
- Secure inter-site communication using IPsec VPN
- Enforce least-privilege access with firewall rules
- Validate secure traffic flows between enterprise sites

---

## Network Architecture

The network consists of two geographically separated enterprise sites connected through the public Internet.

### Headquarters (HQ)

- HQ Router
- HQ Firewall 1
- HQ Firewall 2
- HQ VPN Gateway
- DMZ
- Internal Network (10.1.1.0/24)

### Remote Branch

- Remote Router
- Remote Firewall 1
- Remote Firewall 2
- Remote VPN Gateway
- DMZ
- Internal Network (10.2.1.0/24)

### Internet

- Public network
- Public web servers
- VPN tunnel between both sites

---

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4 Addressing
- Static Routing
- IPsec VPN
- Access Control Lists (ACLs)
- Firewall Policy Design
- Interface PAT
- Network Address Translation (NAT)
- Security Policy Database (SPD)

---

## Security Architecture

### Split-Firewall Design

Each site implements two firewall layers:

- **Firewall 1:** Protects the Internet-facing network.
- **Firewall 2:** Protects the internal enterprise network.

This layered approach increases security by separating external and internal security boundaries.

---

## VPN Architecture

A secure IPsec ESP tunnel connects the headquarters and remote office.

Protected traffic:

```
10.1.1.0/24  ⇄  10.2.1.0/24
```

Traffic between these networks is encrypted and transmitted through the VPN without NAT translation.

---

## Network Address Translation

The project implements:

- Interface PAT for outbound Internet access
- No NAT for VPN traffic
- Separate NAT policies for internal and VPN communication

---

## Firewall Policies

Firewall rules enforce:

- HTTP/HTTPS access to public Internet servers
- Secure communication through the VPN tunnel
- Internal network protection
- Deny-by-default security policy

---

## Skills Demonstrated

### Enterprise Networking

- Enterprise topology design
- Static routing
- IP subnet planning
- Multi-site networking

### Network Security

- Split-firewall architecture
- Access Control Lists (ACLs)
- Security Policy Database (SPD)
- Layered security design
- Least-privilege access control

### VPN Technologies

- Site-to-site IPsec VPN
- Secure branch connectivity
- VPN traffic protection
- Secure enterprise communications

### Network Translation

- Interface PAT
- NAT policy design
- Public/private address translation

### Documentation

- Static route planning
- Firewall ruleset development
- NAT specification
- Security policy documentation

---

## Repository Structure

```text
Enterprise-Split-Firewall-Network/
│
├── README.md
├── Split-FW-Network.pkt
├── Lab5-Answers.pdf
├── Static-Routes.xlsx
├── Security-Policy-Database.xlsx
├── NAT-Rules.xlsx
├── Firewall-Rules.xlsx
```

---

## Testing Performed

The implementation was validated through:

- Static route verification
- VPN traffic validation
- NAT translation testing
- HTTP/HTTPS Internet access
- Inter-site communication testing
- Firewall policy verification
- Packet capture analysis using Simulation Mode

---

## Learning Outcomes

This project provided practical experience designing a secure enterprise network using a layered defense architecture. It reinforced concepts related to enterprise routing, firewall policy design, NAT/PAT implementation, IPsec VPN connectivity, and secure communication between geographically separated sites. The project also strengthened my understanding of how multiple security technologies integrate to protect enterprise infrastructure.

---

## Future Improvements

Potential enhancements include:

- Dynamic routing with OSPF
- High Availability (HSRP/VRRP)
- Certificate-based VPN authentication
- Intrusion Detection/Prevention (IDS/IPS)
- Centralized authentication with RADIUS or TACACS+
- Network monitoring using Syslog and SNMP
- DMVPN for scalable branch connectivity

---

## Author

**Sukaina Hussain**

**B.S. Cybersecurity**  
DePaul University

GitHub: https://github.com/sukaina-h
