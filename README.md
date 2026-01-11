# RIP Routing Using Cisco Packet Tracer

##  Project Overview
This project demonstrates the configuration of **dynamic IP routing using RIP (Routing Information Protocol)** in Cisco Packet Tracer.  
Two routers exchange routing information dynamically, allowing communication between multiple LANs.

---

##  Concepts Used
- RIP (Routing Information Protocol)
- Dynamic Routing
- IP Addressing
- Router & Switch Configuration
- LAN to LAN Communication

---

##  Network Topology
- 2 Routers (Cisco 2811)
- 2 Switches (Cisco 2960)
- 4 PCs
- 3 Networks:
  - 192.168.1.0/24
  - 192.168.2.0/24
  - 192.168.3.0/24 (Router-to-Router)

---

##  Configuration Summary

### PC IP Configuration
| PC | IP Address | Subnet Mask | Default Gateway |
|----|-----------|-------------|----------------|
| PC0 | 192.168.1.2 | 255.255.255.0 | 192.168.1.4 |
| PC1 | 192.168.1.3 | 255.255.255.0 | 192.168.1.4 |
| PC2 | 192.168.2.2 | 255.255.255.0 | 192.168.2.4 |
| PC3 | 192.168.2.3 | 255.255.255.0 | 192.168.2.4 |

---

### RIP Configuration

#### Router 0
router rip
version 2
network 192.168.1.0
network 192.168.3.0


#### Router 1
router rip
version 2
network 192.168.2.0
network 192.168.3.0


---

##  Result
- Successful communication between:
  - PC0 ↔ PC2
  - PC1 ↔ PC3
- Routing tables updated dynamically using RIP.

---

##  Files Included
- `.pkt` Cisco Packet Tracer file
- Network topology screenshots
- Configuration screenshots

---

##  Tools Used
- Cisco Packet Tracer
- GitHub

---

##  Author
**Saloni Pavaskar**
