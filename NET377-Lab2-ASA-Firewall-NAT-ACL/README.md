# NET377 Lab 2 – Cisco ASA Firewall, NAT, and Access Control

## Overview

This repository contains my solution for **NET377 Lab 2**, completed using Cisco Packet Tracer.

The lab focuses on configuring a Cisco ASA firewall to secure a small enterprise network by implementing Network Address Translation (NAT), Access Control Lists (ACLs), secure remote management with SSH, and controlled access to internal and public services.

---

## Objectives

- Configure Cisco ASA firewall interfaces
- Configure static routing
- Implement Interface PAT
- Configure Static NAT
- Configure inbound and outbound ACLs
- Enable SSH remote management
- Verify HTTP and HTTPS services
- Test network connectivity and security policies

---

## Network Topology

```
                    Internet
                        |
                 Internet Router
                        |
                 ----------------
                 |              |
             Cisco ASA      Public Router
                 |               |
          Internal LAN      Public Network
         ------------      --------------
         |          |       |            |
    GZ-Client   GZ-Server  Public Server
```

---

## Technologies Used

- Cisco Packet Tracer
- Cisco ASA 5506-X Firewall
- Cisco IOS
- IPv4 Addressing
- Static Routing
- Network Address Translation (PAT & Static NAT)
- Access Control Lists (ACLs)
- SSH
- HTTP / HTTPS

---

## Skills Demonstrated

### Firewall Configuration

- ASA interface configuration
- Security levels
- Interface naming
- Default routing

### Network Address Translation

- Dynamic PAT for internal clients
- Static NAT for public web access
- Public-to-private address translation

### Access Control

- Extended ACL creation
- Inbound and outbound filtering
- Service-specific access control
- Default deny policy

### Secure Remote Management

- Local user authentication
- SSH configuration
- RSA key generation
- Secure administrative access

### Network Verification

- Routing verification
- NAT verification
- ACL testing
- Connectivity testing
- HTTP and SSH validation

---

## Network Security Features

### Dynamic PAT

Allows internal clients to securely access external networks using the ASA outside interface address.

### Static NAT

Publishes the internal web server to the public Internet while hiding its private IP address.

### Access Control Lists

Configured ACLs enforce security policies including:

- Blocking unauthorized HTTP access
- Allowing approved web traffic
- Restricting SSH access
- Controlling ICMP traffic
- Denying all unspecified traffic

---

## Testing Performed

- Verified interface configurations
- Verified routing tables
- Tested end-to-end connectivity
- Verified PAT operation
- Verified Static NAT operation
- Tested HTTP connectivity
- Tested SSH connectivity
- Validated ACL rules
- Confirmed expected permit and deny behavior

---

## Learning Outcomes

Through this lab I learned how to:

- Configure a Cisco ASA firewall
- Implement dynamic PAT and static NAT
- Design and apply firewall ACLs
- Secure enterprise networks using least-privilege principles
- Configure SSH for secure device management
- Validate firewall policies through connectivity testing
- Troubleshoot firewall and routing configurations

---

## Repository Structure

```
NET377-Lab2-ASA-Firewall-NAT-ACL
│
├── README.md
├── Lab2-Sukaina-Hussain.pkt
├── Lab2-Answers.pdf
└── Lab2-Ruleset-Specifications.xlsx
```

---

## Key Networking Concepts

- Cisco ASA Firewall
- Private vs Public Addressing
- Interface PAT
- Static NAT
- ACL Processing
- Stateful Firewall Concepts
- SSH Remote Administration
- Enterprise Network Security

---

## Author

**Sukaina Hussain**

BS Cybersecurity | DePaul University

GitHub: https://github.com/sukaina-h
