# Enterprise-Network-Security-ACL

Enterprise network security project using VLANs, Inter-VLAN Routing, DHCP, Server, and Extended ACLs in Cisco Packet Tracer.

---


Enterprise network security project implemented in Cisco Packet Tracer.

This project demonstrates VLAN segmentation, Inter-VLAN Routing, DHCP services, and Extended Access Control Lists (ACLs) to isolate the Guest VLAN while allowing authorized communication between internal departments.

---

## Project Overview

The network consists of three departments connected through a Layer 2 switch and a Router-on-a-Stick architecture.

- HR Department (VLAN 10)
- IT Department (VLAN 20)
- Guest Department (VLAN 30)

A central server provides network services, while an Extended ACL protects internal resources from unauthorized Guest access.

---

## Network Topology

![Network Topology](Topology.jpeg)

---

## Features

- VLAN Segmentation
- Inter-VLAN Routing (Router-on-a-Stick)
- 802.1Q Trunk Configuration
- DHCP Configuration
- DNS Server
- HTTP Server
- Extended ACL Security
- Guest VLAN Isolation

---

## IP Addressing

| VLAN | Department | Network | Gateway |
|------|------------|---------|---------|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Guest | 192.168.30.0/24 | 192.168.30.1 |

---

## Server Information

| Device | IP Address | VLAN | Services |
|--------|------------|------|----------|
| SRV1 | 192.168.20.10 | VLAN 20 | DNS, HTTP |

---

## Security Policy (Extended ACL)

| VLAN | Access Policy |
|------|---------------|
| Guest (30) | Cannot access HR VLAN |
| Guest (30) | Cannot access IT VLAN |
| Guest (30) | Cannot access Server |
| HR (10) | Full communication allowed |
| IT (20) | Full communication allowed |

---

## Verification

- ✅ VLANs Configured
- ✅ 802.1Q Trunk Enabled
- ✅ Inter-VLAN Routing Working
- ✅ DHCP Working
- ✅ Extended ACL Implemented
- ✅ Guest VLAN Successfully Isolated

---

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS
- VLAN
- 802.1Q Trunking
- Router-on-a-Stick
- DHCP
- DNS
- HTTP
- Extended Access Control Lists (ACL)

---

## Author

Rawan Alqahtani
