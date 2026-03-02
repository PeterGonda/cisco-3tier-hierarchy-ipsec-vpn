# Enterprise Network Design: 3-Tier Hierarchy & Secure WAN Connectivity
## 📌 Project Overview
This project features a comprehensive design and implementation of a corporate network infrastructure spanning two geographically distant branch offices. The primary objective was to engineer a scalable, highly available, and secure network environment based on industry-standard Cisco hierarchical methodologies.

The project was developed as a graduation thesis at SSOSTA Poprad using the Cisco Packet Tracer simulation platform.

## 🛠 Technical Stack & Implemented Technologies
Network Architecture: 3-Tier Cisco Hierarchical Model consisting of Core, Distribution, and Access layers to ensure modularity and performance.

WAN Connectivity: Established secure site-to-site connectivity using multiple GRE over IPsec VPN tunnels to protect data in transit.

Routing Protocols: Implementation of EIGRP for dynamic routing alongside strategic static routing for specific network segments.

High Availability (HA): Deployment of HSRP (First Hop Redundancy Protocol) for gateway redundancy and L2/L3 EtherChannel (using LACP/PAgP) for link aggregation and increased bandwidth.

Network Security: Advanced security measures including Extended Access Control Lists (ACLs), Port Security for MAC-level protection, and encrypted device management via SSH.

IP Addressing: Detailed and optimized IP addressing scheme designed using VLSM (Variable Length Subnet Masking) to minimize address waste.

L2 Technologies: Comprehensive VLAN segmentation, 802.1Q Trunking, and STP/PVST+ for a loop-free topology.

## 🏗 Key Architectural Features
Redundancy and Failover: The HSRP configuration provides a seamless failover mechanism for the default gateway, ensuring business continuity during distribution switch failures. EtherChannel further enhances link-level resilience.

Secure WAN Tunneling: All inter-branch traffic is encapsulated and encrypted via IPsec, maintaining the integrity and confidentiality of sensitive corporate data across simulated public infrastructure.

Logical Segmentation: The infrastructure is logically partitioned into distinct VLANs (e.g., Management, Servers, Users) to improve both security posture and administrative efficiency.

Granular Access Policy: Extended ACLs are meticulously configured to enforce the principle of least privilege, restricting network access based on administrative roles and segment requirements.

## 📂 Repository Structure
/topology: Contains the primary .pkt (Cisco Packet Tracer) simulation file.

/docs: Includes the full technical documentation and graduation thesis report in PDF and DOCX formats.

/configs: Text-based configuration files exported from key network devices for review.

## 🚀 How to Use
Download and install Cisco Packet Tracer (version 8.x recommended).

Open the project file located in the /topology directory.

Allow the network protocols (STP, EIGRP) to converge.

Verify connectivity using ping or by simulating HTTP traffic between the branch offices.
