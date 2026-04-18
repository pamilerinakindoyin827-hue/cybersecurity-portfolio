# Secure WAN Architecture – Branch Connectivity (Ghana & Cape Verde)

## Overview
This project demonstrates the design and implementation of a secure Wide Area Network (WAN) connecting two branch offices located in Ghana and Cape Verde using Cisco Packet Tracer.

The objective was to simulate real-world enterprise network connectivity while enforcing security policies through Access Control Lists (ACLs).

---

## Objectives
- Design a WAN topology connecting two remote branch networks  
- Implement CIDR-based IP addressing for efficient subnetting  
- Configure routing for inter-branch communication  
- Apply Access Control Lists (ACLs) for traffic control  
- Restrict network traffic to only HTTP and ICMP protocols  

---

## 🛠️ Tools & Technologies
- Cisco Packet Tracer  
- TCP/IP Networking  
- CIDR Subnetting  
- Access Control Lists (ACLs)  
- Routing Protocol Concepts  

---

## Implementation

### 1. Network Design
- Designed a WAN topology connecting two geographically separated branch networks  
- Assigned IP addresses using CIDR-based subnetting  
- Configured routers and interfaces to enable inter-network communication  

### 2. Routing Configuration
- Established end-to-end connectivity between both branch networks  
- Verified routing functionality using ICMP (ping tests)  

### 3. Security Implementation
- Implemented Access Control Lists (ACLs) to enforce security policies  
- Configured rules to allow only:
  - HTTP (web traffic)  
  - ICMP (ping/testing traffic)  
- Blocked all other unnecessary traffic to reduce attack surface  

### 4. Testing & Validation
- Performed connectivity tests between both branches  
- Verified allowed traffic successfully passed through the network  
- Confirmed that restricted traffic was properly denied  

---

## Security Insights
- ACLs are an effective method for enforcing network-level security policies  
- Limiting traffic reduces potential attack vectors and exposure  
- Proper network segmentation improves security monitoring and control  
- Simulated environments help validate security configurations before real deployment  

---

## Evidence
Include screenshots such as:
- Network topology diagram  
- Router configuration (ACL rules)  
- Successful ping tests between branches  
- Packet Tracer simulation view  

---

## Conclusion
This project demonstrates practical experience in secure network design, traffic filtering, and enterprise WAN configuration using Cisco Packet Tracer. It reflects foundational skills in network security and controlled communication between distributed systems.
