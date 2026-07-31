# Cisco IPSec Site-to-Site VPN

> A Cisco IOS implementation of a site-to-site IPsec VPN connecting two private enterprise networks over an untrusted public network. The project demonstrates secure communication using ISAKMP/IKE Phase 1, IPsec ESP, pre-shared key authentication, and AES-256 encryption.

---

## Overview

This project implements a secure site-to-site Virtual Private Network (VPN) between two enterprise branch offices using Cisco IOS routers in Packet Tracer.

The VPN encrypts traffic exchanged between two private LANs while allowing communication across a simulated public network. The implementation follows enterprise VPN design principles by using IKE Phase 1 for tunnel establishment and IPsec ESP for encrypted data transport.

---

## Project Objectives

- Build a secure site-to-site VPN
- Configure ISAKMP (IKE Phase 1)
- Configure IPsec ESP
- Authenticate peers using a pre-shared key
- Encrypt traffic using AES-256
- Protect data integrity with SHA
- Secure communication between private LANs
- Validate encrypted communication through VPN testing

---

## Network Topology

The topology consists of two enterprise sites connected over a simulated public WAN.

### Site 1

- Router R1
- Switch
- PC1
- Private LAN: **10.0.19.0/24**

### Site 2

- Router R2
- Switch
- PC2
- Private LAN: **192.168.19.0/24**

### Public Network

- Serial WAN Link
- Network: **172.30.2.0/30**

Traffic between the two private networks is encrypted using an IPsec tunnel.

---

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4 Addressing
- Static Routing
- ISAKMP (IKE Phase 1)
- IPsec ESP
- AES-256 Encryption
- SHA Hashing
- Diffie-Hellman Group 5
- Access Control Lists (ACLs)

---

## VPN Configuration

### IKE Phase 1

The VPN peers negotiate secure communication using:

- AES-256 encryption
- SHA hashing
- Pre-Shared Key authentication
- Diffie-Hellman Group 5

### IKE Phase 2

IPsec Security Associations are established using:

- ESP Encryption
- ESP SHA-HMAC authentication

---

## Interesting Traffic

Only traffic between the private enterprise networks is encrypted.

```
10.0.19.0/24  ⇄  192.168.19.0/24
```

ACLs identify this traffic for VPN encapsulation.

---

## Security Features

### Encryption

- AES-256

### Integrity

- SHA

### Authentication

- Pre-Shared Key

### Key Exchange

- Diffie-Hellman Group 5

### Secure Tunnel

- IPsec ESP

---

## Skills Demonstrated

### Networking

- IPv4 addressing
- Static routing
- WAN connectivity
- Cisco IOS configuration

### Network Security

- Site-to-site VPN deployment
- IPsec configuration
- ISAKMP policy creation
- Secure key exchange
- Traffic encryption
- Access Control Lists

### Troubleshooting

- VPN tunnel verification
- Security Association validation
- End-to-end connectivity testing
- Tunnel traffic verification

---

## Repository Structure

```text
Cisco-IPSec-Site-to-Site-VPN/
│
├── README.md
├── IPSec-Site-to-Site-VPN.pkt
├── Lab4-Answers.pdf
└── Device-Configurations/
    ├── R1.txt
    └── R2.txt
```

---

## Testing Performed

The VPN implementation was validated through:

- LAN-to-LAN connectivity testing
- End-to-end ICMP testing
- Tunnel establishment verification
- Security Association (SA) verification
- Successful encrypted communication between private subnets

---

## Learning Outcomes

This project provided hands-on experience designing and implementing a site-to-site IPsec VPN using Cisco IOS. It reinforced concepts related to secure enterprise connectivity, VPN tunnel establishment, cryptographic protocols, traffic encryption, and secure communication across untrusted networks.

---

## Future Improvements

Possible enhancements include:

- Dynamic routing (OSPF) over the VPN
- Certificate-based authentication
- GRE over IPsec
- Redundant VPN tunnels
- High Availability (HSRP)
- DMVPN implementation
- Remote Access VPN

---

## Author

**Sukaina Hussain**

**B.S. Cybersecurity**  
DePaul University

GitHub: https://github.com/sukaina-h
