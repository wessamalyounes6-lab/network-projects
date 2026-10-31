# Cisco Packet Tracer Lab: OSPF, DHCP & SSH Configuration

## Overview
This repository contains a Cisco Packet Tracer network simulation (`.pkt`) demonstrating core enterprise networking concepts, including dynamic routing, automatic IP address allocation, and secure remote management.

## Network Architecture & Features
- **Dynamic Routing (OSPF):** Configured Open Shortest Path First protocol for efficient, scalable inter-router communication.
- **Dynamic Addressing (DHCP):** Implemented DHCP pool services to automatically assign IP addresses, subnet masks, and default gateways to end devices.
- **Secure Remote Access (SSH):** Configured SSH on network devices (routers/switches) with encrypted credentials for secure administrative access, disabling insecure Telnet.

## Topology Files
- `dhcp.ospf.ssh.pkt`: Primary Packet Tracer topology file containing the full configuration and tested network devices.

## How to Test the Topology
1. Open `dhcp.ospf.ssh.pkt` in **Cisco Packet Tracer**.
2. Verify dynamic IP assignment on PCs via DHCP (`ipconfig` in command prompt).
3. Test end-to-end connectivity using `ping` across different subnets/OSPF areas.
4. Verify SSH access from a client PC to the router/switch CLI:
   ```bash
   ssh -l <username> <device-ip>

