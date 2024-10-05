# Network-Configuration-VLSM-PacketTracer
(![Topology](https://github.com/user-attachments/assets/a37fda52-8b46-4a14-8675-ebada76d8c76))

## Project Description
This project demonstrates the design and configuration of a computer network using **Cisco Packet Tracer**, with the primary focus on **VLSM (Variable Length Subnet Masking)** to optimize IP address allocation. The network topology includes routers, switches, PCs, and servers, all configured to ensure full connectivity and functionality. Key services like **DNS** and **HTTP** have been set up, with static routing implemented across the network for efficient communication.

## Project Objectives
The main objectives of this project are:
- Design a network topology with appropriate devices.
- Use VLSM for IP address segmentation across different LAN and WAN segments.
- Configure routers, switches, servers, and PCs with necessary settings.
- Implement static routing to ensure all devices can communicate.
- Set up DNS and HTTP services, including a simple web page hosted on the HTTP server.
- Verify full network connectivity and functionality using various network tools.

## Topology Overview
The network topology includes the following segments:
- **LAN 1**: Large networks for client PCs.
- **LAN 2**: Medium to small networks for specialized services.
- **WAN**: Used to interconnect routers across different geographical locations.

Each LAN and WAN has been subnetted using VLSM to optimize the IP address space based on the number of required hosts.

## Key Features
1. **Device Configuration**: 
   - All routers, switches, servers, and PCs have been properly named and cabled according to the provided topology.
   - Password protection has been added for both console and vty access on routers, with `FCIT` as the password and `lab` as the enable secret.
   
2. **VLSM Subnetting**:
   - IP addresses are assigned using VLSM to meet the exact requirements of each LAN and WAN.
   - The router interfaces use the first available IP in the subnet, and server interfaces use the last available IP.
   
3. **DHCP Setup**:
   - DHCP is configured on the **SANA1** router to dynamically assign IP addresses to PCs in **LAN2**.

4. **Static Routing**:
   - Static routing has been implemented on all routers to ensure full network connectivity.

5. **DNS and HTTP Server**:
   - The DNS server is configured to resolve the domain **www.FCIT.com** to the IP address `210.200.100.130`.
   - The HTTP server hosts a simple web page that displays a success message and personal details.

## Configuration Details
### Devices:
- **Routers**: Configured with VLSM-based subnets, static routing, and secure access.
- **Switches**: Used to connect LAN segments.
- **Servers**: Configured as DNS and HTTP servers.
- **PCs**: Connected to LAN segments, configured with static or dynamic IPs.

### IP Addressing:
- Subnets are created for each LAN and WAN segment using VLSM, ensuring efficient use of the available address space.

## How to Use
1. Open the project in **Cisco Packet Tracer**.
2. Verify all configurations by testing connectivity between devices.
3. On any PC, use the web browser to access **www.FCIT.com** and confirm the success message.
4. Review static routing settings on the routers to understand how inter-network communication is achieved.

## Conclusion
This project successfully demonstrates the use of VLSM to create an efficient IP addressing scheme, along with configuring essential network services such as DNS and HTTP. The network has been fully tested and is operational, providing an excellent foundation for understanding network design principles.

---


