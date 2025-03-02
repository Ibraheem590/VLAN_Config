
# VLAN Configuration and Inter-VLAN Routing

## Project Overview

This project demonstrates the configuration of **VLANs** and **Inter-VLAN Routing** using **Cisco devices**. The network topology includes both a **Layer 2 switch** and a **Layer 3 switch** to illustrate the differences in VLAN handling, routing capabilities, and traffic management. 

### **Objective**:  
- To configure **VLANs** on a **Layer 2 switch** and show that devices on different VLANs cannot communicate without routing.
- To configure **Inter-VLAN Routing** using a **Layer 3 switch** and allow devices on different VLANs to communicate.

---

## Network Topology

- **Devices**:
  - **PC1** (VLAN 10: Sales) → 192.168.10.10
  - **PC2** (VLAN 20: HR) → 192.168.20.10
  - **Layer 2 Switch** (for VLAN configurations)
  - **Layer 3 Switch** (for Inter-VLAN Routing)
  - **Router** (only used in Layer 2 scenario for Router-on-a-Stick)
  
- **VLANs**:
  - **VLAN 10 (Sales)**: 192.168.10.0 /24
  - **VLAN 20 (HR)**: 192.168.20.0 /24

---

## Files Included

- **VLAN Configuration File** (`vlan-config.txt`): This file contains all the necessary configuration commands to set up VLANs on the switches.
- **Inter-VLAN Routing Packet Tracer File** (`inter-vlan-routing.pkt`): Packet Tracer file demonstrating the working Inter-VLAN Routing configuration using a Layer 3 Switch.
- **Layer 2 Configuration Packet Tracer File** (`layer-2.pkt`): Packet Tracer file for the Layer 2 setup using **Router-on-a-Stick** for Inter-VLAN Routing.

---

## Configuration Steps

### 1. **Layer 2 Switch Configuration (Without Routing)**

In this scenario, the **Layer 2 switch** is used to configure the VLANs, and the router handles the Inter-VLAN routing.

- Configure VLANs 10 and 20 on the Layer 2 switch.
- Assign switch ports to the appropriate VLANs.
- Set up **Router-on-a-Stick** for routing between VLANs.

For detailed configuration commands, refer to the **vlan-config.txt** file.

### 2. **Layer 3 Switch Configuration (With Inter-VLAN Routing)**

A **Layer 3 switch** is used in this scenario, with **SVIs (Switched Virtual Interfaces)** configured to enable routing between VLANs.

- Enable **IP routing** on the Layer 3 switch.
- Create **SVIs** for VLAN 10 and VLAN 20.
- Assign IP addresses to each SVI (e.g., 192.168.10.1 for VLAN 10 and 192.168.20.1 for VLAN 20).
- Assign switch ports to VLANs and enable routing to allow inter-VLAN communication.

For the full configuration, refer to the **vlan-config.txt** file.

## How to Use

1. Open the **Packet Tracer files** to visualize the network topology.
2. Apply the **vlan-config.txt** configuration to the switches.
3. Test connectivity:
   - In the **Layer 2 switch** setup, test the connectivity between the two PCs.
   - In the **Layer 3 switch** setup, test inter-VLAN communication.
   
---

## Requirements

- **Cisco Packet Tracer** version 7.0 or higher.
- Basic understanding of **VLANs**, **Layer 2 switches**, and **Layer 3 switches**.
- Understanding of **IP Routing** concepts.


## Author

**Ibraheem590**

Feel free to reach out if you have any questions or suggestions for improvement!


## Contributions

Contributions are welcome! Please open an issue or submit a pull request if you'd like to contribute.


