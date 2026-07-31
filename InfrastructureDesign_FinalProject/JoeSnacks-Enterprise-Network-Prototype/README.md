# Enterprise Network Design Prototype

> A prototype enterprise network designed and secured as part of the NET377 Network Security course. This project demonstrates the complete lifecycle of building an enterprise network—from initial architecture and routing to implementing layered firewall security controls.

---

## Overview

This repository contains the final implementation of an enterprise network prototype developed for the **Joe Snacks Design Project**. The project simulates a secure enterprise environment with segmented networks, public-facing services, internal infrastructure, and controlled communication between security zones.

The prototype was developed in two phases:

- **Phase 1 (Lab 3):** Designed and implemented the enterprise network architecture, IP addressing plan, static routing, and NAT.
- **Phase 2 (Lab 6):** Expanded the prototype by implementing firewall policies, access control lists (ACLs), and secure communication between network segments.

The repository contains the **final prototype**, which incorporates both networking and security components.

---

## Project Objectives

- Design a secure enterprise network architecture
- Implement network segmentation using multiple security zones
- Configure static routing between enterprise networks
- Implement Network Address Translation (NAT)
- Secure network traffic using Access Control Lists (ACLs)
- Restrict communication according to enterprise security policies
- Validate connectivity and security through testing

---

## Network Architecture

The enterprise network consists of multiple security zones designed to isolate resources while allowing only authorized communication.

### Internet

- Internet Router
- External Users
- Public Web Server

### Red Network (DMZ)

- Red Edge Router
- Firewall R1
- Firewall R2
- DMZ Switch
- JS Sales Server
- Remote Desktop Gateway

### Green Network (Internal)

- Green Edge Router
- Firewall G1
- Firewall G2
- Intranet Layer 3 Switch
- Active Directory Server
- Database Server
- HR Server
- Web Security Appliance (WSA)
- Internal Users

---

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- IPv4 Addressing
- Static Routing
- Layer 3 Switching
- Network Address Translation (NAT)
- Access Control Lists (ACLs)
- Enterprise Firewall Policies
- HTTP / HTTPS
- Remote Desktop Protocol (RDP)

---

## Project Evolution

### Phase 1 – Enterprise Network Prototype (Lab 3)

The initial prototype established the enterprise infrastructure by implementing:

- Enterprise topology design
- IP subnet planning
- IP addressing
- Static routing
- Layer 3 switching
- NAT configuration
- End-to-end connectivity validation
- Traffic flow verification

### Phase 2 – Security Implementation (Lab 6)

The prototype was enhanced with security controls, including:

- Firewall deployment
- Access Control Lists (ACLs)
- Security zone segmentation
- Service-specific filtering
- Least-privilege communication policies
- Enterprise firewall rule implementation
- Secure routing between network segments

---

## Security Features

### Network Segmentation

The enterprise network is divided into multiple security zones:

- Internet
- DMZ
- Internal Network
- Intranet Services

Segmentation limits lateral movement and isolates critical enterprise resources.

### Firewall Policies

Firewall rules control traffic between:

- Internet ↔ DMZ
- DMZ ↔ Internal Network
- Internal Users ↔ Enterprise Services
- Internal Users ↔ Internet

Only explicitly permitted traffic is allowed between zones.

### Network Address Translation (NAT)

The project implements NAT to:

- Publish public-facing services
- Protect private internal addresses
- Support secure communication between internal and external networks

---

## Enterprise Services

### DMZ

- JS Sales Server
- Remote Desktop Gateway

### Internal Services

- Active Directory Server
- Database Server
- HR Server
- Web Security Appliance (WSA)

### Client Networks

- Internal Users
- External Employees
- Internet Customers

---

## Skills Demonstrated

### Enterprise Networking

- Enterprise network design
- IP addressing and subnet planning
- Static routing
- Layer 3 switching
- Enterprise topology implementation

### Network Security

- Firewall deployment
- Access Control List (ACL) configuration
- Security zone design
- Network segmentation
- Least-privilege access control

### Network Services

- Network Address Translation (NAT)
- HTTP / HTTPS connectivity
- Remote Desktop access
- Enterprise traffic management

### Troubleshooting & Validation

- Connectivity testing
- Routing verification
- Firewall rule validation
- Traffic flow analysis
- End-to-end network testing

---

## Repository Structure

```text
Enterprise-Network-Design-Prototype/
│
├── README.md
├── Enterprise-Network-Prototype.pkt
├── Lab6-Answers.pdf
├── IP-Addressing-Specifications.xlsx
├── IP-Subnet-Plan.xlsx
├── Firewall-Rules-Specifications.xlsx
├── Static-Routes-Specifications.xlsx
├── NAT-Rules-Specifications.xlsx
└── Device-Configurations/
    ├── FW-R1.txt
    ├── FW-R2.txt
    ├── FW-G1.txt
    ├── FW-G2.txt
    ├── Rtr-Red.txt
    ├── Rtr-Green.txt
    ├── Internet.txt
    ├── SW-DMZ.txt
    └── SW-Intranet.txt
```

---

## Learning Outcomes

This project strengthened my understanding of enterprise networking by demonstrating how multiple technologies work together to build a secure infrastructure. Through the design and implementation process, I gained hands-on experience with:

- Designing enterprise network topologies
- Planning IP addressing and subnet allocation
- Configuring static routing
- Implementing Network Address Translation (NAT)
- Creating and applying firewall access control policies
- Enforcing network segmentation
- Securing communication between enterprise services
- Testing and validating enterprise network functionality

---

## Future Improvements

Potential enhancements to this prototype include:

- Dynamic routing using OSPF
- VLAN implementation
- Site-to-site VPN connectivity
- High Availability (HSRP/VRRP)
- Intrusion Detection and Prevention (IDS/IPS)
- Network monitoring with Syslog and SNMP
- AAA authentication with RADIUS or TACACS+
- Centralized logging and security monitoring

---

## Author

**Sukaina Hussain**

**B.S. Cybersecurity**  
DePaul University

GitHub: https://github.com/sukaina-h
