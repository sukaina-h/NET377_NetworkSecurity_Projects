# NET377 Lab 1 – Static Routing, HTTP, and SSH Configuration

## Overview

This repository contains my solution for **NET377 Lab 1**, where I configured a small enterprise network in Cisco Packet Tracer.

The lab focused on configuring router interfaces, implementing static routing, enabling HTTP and SSH services, and verifying end-to-end connectivity across multiple networks.

---

## Network Topology

```
Corporate LAN
-----------------------------
GZ-Client
      |
   Switch
   /     \
Server   GZ-CE Router
            |
         Internet Router
            |
       Public Router
       Loopback 2.2.2.2
```

---

## Objectives

- Configure IPv4 addressing
- Configure router hostnames
- Configure static routing
- Configure default routes
- Enable HTTP service
- Configure SSH remote management
- Verify end-to-end connectivity

---

## Technologies Used

- Cisco Packet Tracer 8.2+
- Cisco IOS
- IPv4 Addressing
- Static Routing
- SSH
- HTTP
- CLI Configuration

---

## Skills Demonstrated

### Network Configuration

- Interface configuration
- IPv4 subnetting
- Default gateway configuration
- Static route implementation
- Router verification

### Network Services

- HTTP server configuration
- SSH server configuration
- Local user authentication
- RSA key generation
- Secure remote management

### Verification & Troubleshooting

- Ping testing
- Telnet testing
- SSH testing
- Route verification
- Interface verification

---

## Router Configuration Highlights

### GZ-CE

- Configured LAN and WAN interfaces
- Configured default route toward ISP

### Internet Router

Configured static routes for:

- Corporate LAN
- Public Router loopback

### Public Router

Configured:

- Local user authentication
- Domain name
- RSA keys
- SSH access
- Default route

---

## Testing Performed

✔ Interface verification using

```
show ip interface brief
```

✔ Static routing verification

```
show ip route
```

✔ End-to-end ICMP connectivity

```
ping
```

✔ HTTP connectivity

```
telnet <Server-IP> 80
```

✔ SSH connectivity

```
ssh -l Lab1 2.2.2.2
```

---

## Learning Outcomes

Through this lab I learned how to:

- Configure Cisco routers from scratch
- Implement static routing across multiple networks
- Configure secure remote administration using SSH
- Enable and verify HTTP services
- Validate routing tables and interface status
- Troubleshoot network connectivity using Cisco IOS commands

---

## Repository Structure

```
NET377-Lab1-Static-Routing-SSH-HTTP
│
├── README.md
├── Lab1-Sukaina-Hussain-v1.pkt
├── Lab1-Answers.pdf
└── screenshots/
    ├── topology.png
    ├── ping-tests.png
    ├── show-ip-route.png
    ├── ssh-login.png
    └── http-test.png
```

---

## Author

**Sukaina Hussain**

BS Cybersecurity | DePaul University

GitHub: https://github.com/sukaina-h
