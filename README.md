# Small Enterprise Network Design & Implementation

## Description
This project showcases the design and implementation of a **Small Enterprise Network** for a company called **AlphaTech**. The solution is built to be **secure**, **scalable**, and **resilient**. It features **VLAN segmentation**, **OSPF routing**, **NAT configurations**, **High Availability (HSRP)**, and various **network security measures**. The solution was designed to meet the needs of a small-to-medium-sized business, ensuring efficiency, performance, and secure communication between internal systems.

The project was created based on the principles learned during the **CCNA course on Udemy**, demonstrating the ability to design, implement, and troubleshoot network infrastructures using Cisco technologies.

## Objective
The objective of this project is to showcase my skills and knowledge gained from completing the **CCNA course on Udemy**. It involves configuring a resilient network infrastructure with features such as:

- **VLAN Segmentation** for secure data separation.
- **OSPF Routing** for dynamic and efficient routing across the network.
- **High Availability** through **HSRP** to ensure network continuity.
- **Syslog Configuration** for network monitoring and logging.

## Network Infrastructure Overview
The network infrastructure consists of several core components:
1. **Edge Routers**: HO-RT01 and HO-RT02 for external connectivity.
2. **Core Switches**: Core_SW01 and Core_SW02 for VLAN routing and redundancy.
3. **Access Switches**: Access_SW01, Access_SW02, Access_SW03 for user connectivity.

### Key Features
- **Edge Routers**: Provide internet access, implement **HSRP** for failover, and **NAT** for internal IP address translation.
- **Core Switches**: Support **OSPF** routing, VLAN trunking, and inter-VLAN routing.
- **Access Switches**: Secure user access, implement **DHCP Snooping**, **Port Security**, and **VLAN Segmentation**.

## Technologies Used
- **Cisco Packet Tracer**: Used for simulating and testing network configurations.
- **Cisco IOS**: Router and switch operating system used for configuration.
- **VLANs**: Network segmentation to enhance security and manage traffic efficiently.
- **OSPF**: Dynamic routing protocol for optimal path selection across routers.
- **HSRP**: High availability protocol for redundant routing.
- **Syslog**: Network monitoring and event logging.

## Network Design & Configuration

### 1. **Edge Routers**: HO-RT01 and HO-RT02
- **SSH Remote Access**: Configured with domain `alphatech.local` and RSA key support for secure administrative access.
- **NAT Configuration**: Translates internal IP addresses to public IPs.
- **High Availability (HSRP)**: Ensures redundancy for the **virtual gateway**.
- **Routing**: Configured with **OSPF** for dynamic routing across the network.

### 2. **Core Switches**: Core_SW01 and Core_SW02
- **VLAN Configuration**: Implemented **802.1Q trunking** for inter-VLAN communication.
- **Routing Protocols**: **OSPF** is used for dynamic routing between VLANs and for redundancy.
- **Security**: **SSH** access and **ACLs** are used to restrict unauthorised access.
- **High Availability**: **HSRP** is enabled on **SVIs** for redundancy and failover.

### 3. **Access Switches**: Access_SW01
- **Port Security**: Configured with sticky MAC addresses and a violation mode to restrict unauthorised devices.
- **DHCP Snooping**: Ensures that only trusted DHCP servers assign IP addresses.
- **Spanning Tree Protocol**: Enhanced with **PortFast** and **BPDU Guard** for faster convergence.

## Configuration Files
All the configuration files for the network devices are included in the repository. You will find Both Router , Both Core switch and all 3 Access switches running_config.txt
## How to Use

### Prerequisites:
- Install **Cisco Packet Tracer** for network simulation.
- load the Project Master file.pkt
- load the network device with the config files

### Setup Instructions:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Habibur-Rahman192/CCNA-PROJECT.git
