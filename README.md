# 5-VLAN Inter-VLAN Routing Lab

## Overview

This project demonstrates the implementation of a multi-VLAN network using Router-on-a-Stick in Cisco Packet Tracer. Five departments were separated into different VLANs and configured to communicate with each other through inter-VLAN routing.

## Network Topology

The network consists of:

- 1 Router
- 2 Switches
- 10 PCs
- 5 VLANs

### VLAN Structure

| VLAN ID | Department | Gateway |
|----------|----------|----------|
| 10 | Sales | 192.168.50.1 |
| 20 | HR | 192.168.50.65 |
| 30 | IT | 192.168.50.129 |
| 40 | Finance | 192.168.50.193 |
| 50 | Management | 192.168.51.1 |

## Technologies Used

- Cisco Packet Tracer
- VLANs
- Router-on-a-Stick
- IEEE 802.1Q Trunking
- Subnetting
- Inter-VLAN Routing
- Spanning Tree Protocol (STP)

## Configuration Summary

### Router Configuration

- Created five subinterfaces:
  - GigabitEthernet0/0.10
  - GigabitEthernet0/0.20
  - GigabitEthernet0/0.30
  - GigabitEthernet0/0.40
  - GigabitEthernet0/0.50

- Configured encapsulation using:

```bash
encapsulation dot1Q <VLAN_ID>
```

- Assigned gateway IP addresses to each VLAN.

### Switch Configuration

- Created five VLANs.
- Assigned access ports to each department.
- Configured trunk ports between switches and the router.

## Verification Commands

```bash
show vlan brief
show interfaces trunk
show ip interface brief
show running-config
```

## Troubleshooting

The following issues were encountered during the lab:

- Incorrect interface configuration mode
- Trunk port configuration errors
- Spanning Tree Protocol blocking traffic

The issues were resolved by verifying trunk links and checking STP forwarding states.

## Project Structure

```text
5-VLAN-Inter-VLAN-Routing-Lab/

├── README.md
├── AlexOjo-5Vlan-Lab.pkt

├── configs/
│   ├── router-config.txt
│   ├── switch0-config.txt
│   └── switch1-config.txt

├── screenshots/
│   ├── topology.png
│   ├── ping-test.png
│   ├── router-config.png
│   ├── switch0-vlan.png
│   └── switch1-vlan.png

└── docs/
    ├── subnetting-table.md
    └── troubleshooting.md
```

## Skills Demonstrated

- Network segmentation using VLANs
- Subnetting and IP addressing
- Router-on-a-Stick configuration
- Trunking using IEEE 802.1Q
- Network troubleshooting
- Cisco CLI configuration

---

Created by Alex Ojo
=======
# 5-VLAN Inter-VLAN Routing Lab

## Overview

This project demonstrates the implementation of a multi-VLAN network using Router-on-a-Stick in Cisco Packet Tracer. Five departments were separated into different VLANs and configured to communicate with each other through inter-VLAN routing.

## Network Topology

The network consists of:

- 1 Router
- 2 Switches
- 10 PCs
- 5 VLANs

### VLAN Structure

| VLAN ID | Department | Gateway |
|----------|----------|----------|
| 10 | Sales | 192.168.50.1 |
| 20 | HR | 192.168.50.65 |
| 30 | IT | 192.168.50.129 |
| 40 | Finance | 192.168.50.193 |
| 50 | Management | 192.168.51.1 |

## Technologies Used

- Cisco Packet Tracer
- VLANs
- Router-on-a-Stick
- IEEE 802.1Q Trunking
- Subnetting
- Inter-VLAN Routing
- Spanning Tree Protocol (STP)

## Configuration Summary

### Router Configuration

- Created five subinterfaces:
  - GigabitEthernet0/0.10
  - GigabitEthernet0/0.20
  - GigabitEthernet0/0.30
  - GigabitEthernet0/0.40
  - GigabitEthernet0/0.50

- Configured encapsulation using:

```bash
encapsulation dot1Q <VLAN_ID>
```

- Assigned gateway IP addresses to each VLAN.

### Switch Configuration

- Created five VLANs.
- Assigned access ports to each department.
- Configured trunk ports between switches and the router.

## Verification Commands

```bash
show vlan brief
show interfaces trunk
show ip interface brief
show running-config
```

## Troubleshooting

The following issues were encountered during the lab:

- Incorrect interface configuration mode
- Trunk port configuration errors
- Spanning Tree Protocol blocking traffic

The issues were resolved by verifying trunk links and checking STP forwarding states.

## Project Structure

```text
5-VLAN-Inter-VLAN-Routing-Lab/

├── README.md
├── AlexOjo-5Vlan-Lab.pkt

├── configs/
│   ├── router-config.txt
│   ├── switch0-config.txt
│   └── switch1-config.txt

├── screenshots/
│   ├── topology.png
│   ├── ping-test.png
│   ├── router-config.png
│   ├── switch0-vlan.png
│   └── switch1-vlan.png

└── docs/
    ├── subnetting-table.md
    └── troubleshooting.md
```

## Skills Demonstrated

- Network segmentation using VLANs
- Subnetting and IP addressing
- Router-on-a-Stick configuration
- Trunking using IEEE 802.1Q
- Network troubleshooting
- Cisco CLI configuration

---

Created by Alex Ojo
>>>>>>> f8b229482dd26e4b8ebf74e615f8f3d794af75db
Cybersecurity Student | Networking Enthusiast
