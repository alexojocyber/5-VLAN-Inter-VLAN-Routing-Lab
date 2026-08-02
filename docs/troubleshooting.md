# Troubleshooting

## Problem

Inter-VLAN communication initially failed even though the router subinterfaces and VLAN configurations appeared correct.

## Investigation

The following commands were used:

```bash
show interfaces trunk
show vlan brief
show ip interface brief
show spanning-tree
```

## Root Cause

Spanning Tree Protocol (STP) blocked traffic on the trunk interface, preventing VLAN traffic from reaching the router.

## Solution

The trunk interface was verified and STP forwarding states were checked.

```bash
interface FastEthernet0/5
switchport mode trunk
spanning-tree portfast trunk
```

## Result

Communication between all VLANs was restored successfully.