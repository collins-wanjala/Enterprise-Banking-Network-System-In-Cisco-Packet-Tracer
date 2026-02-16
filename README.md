# Enterprise-Banking-Network-System-In-Cisco-Packet-Tracer

🏦 Secure Enterprise Banking Network System

📌 Project Overview

This project demonstrates the design and implementation of a highly secure, scalable enterprise network infrastructure tailored for a banking environment. It focuses on isolating sensitive financial data, automating IP management via DHCP, and enforcing strict access control through VLAN segmentation.



🎯 Key Objectives

Zero-Trust Architecture: Ensuring that only authorized departments can access the core banking server.



Scalability: Implementing a multi-branch DHCP configuration for seamless device integration.



Redundancy: Reducing single points of failure within the routing switching fabric.



🛠️ Technical Stack

Simulation/Hardware: Cisco Packet Tracer / GNS3 / Physical Cisco Routers



Routing Protocols: OSPF / EIGRP (Edit as per your project)



Security: Standard \& Extended ACLs, Port Security, VLAN Trunking (802.1Q)



Services: DHCP, DNS, NAT/PAT



**2. DHCP Configuration**

To prevent manual IP conflicts and handle high turnover of guest/staff devices:



Exclusion Lists: Core infrastructure IPs (Gateways, Servers) are excluded from the pool.



Lease Optimization: Optimized for high-security environments to recycle IPs frequently.



**3. Security Hardening**

ACLs: Traffic from the Guest VLAN is strictly prohibited from reaching the "Core Database" VLAN.



SSH over Telnet: All remote management is encrypted.



Port Security: MAC-address filtering on switch ports to prevent unauthorized hardware "plug-ins."



🚀 How to Deploy

Clone the Repository:

Bash

https://github.com/collins-wanjala/Enterprise-Banking-Network-System-In-Cisco-Packet-Tracer

Open the Lab: Load the .pkt or .gns3 file in your preferred simulator.



Apply Configurations: Use the provided .txt files in the /configs folder to manually paste configurations into the CLI of the routers and switches.



📊 Results \& Verification

Connectivity: All endpoints can reach the Internet via NAT, but internal VLANs remain isolated.



DHCP Verification: End-user devices successfully receive dynamic IPs within their designated subnet.



Security Audit: Pings from VLAN 20 to the Banking Server (VLAN 10) are successfully dropped by Extended ACLs.

