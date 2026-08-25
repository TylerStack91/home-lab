# pfSense Firewall Lab

## Objective

Build and configure a virtual network using pfSense to practice firewall administration, network segmentation, NAT, remote access, and troubleshooting.

## Environment

- pfSense
- Virtual machines
- Windows
- Linux
- Private virtual network

## Skills Practiced

- TCP/IP networking
- Firewall configuration
- NAT
- Port forwarding
- IP addressing
- Network troubleshooting
- Remote access
- Security fundamentals

## Lab Overview

In this lab, I used pfSense as the firewall/router between systems in a virtual network.

The goal was to understand how traffic moves between systems and how firewall and NAT rules control access to services.
## Network Diagram

```mermaid
flowchart LR
    Internet((Internet))
    FW[pfSense Firewall / Router]
    LAN[Private Lab Network]
    WIN[Windows VM]
    LINUX[Linux VM]

    Internet --> FW
    FW --> LAN
    LAN --> WIN
    LAN --> LINUX
## Troubleshooting Process

When connectivity did not work as expected, I checked:

1. IP address configuration
2. Subnet and default gateway settings
3. Network adapter configuration
4. pfSense firewall rules
5. NAT and port-forwarding rules
6. Whether the destination service was running
7. Connectivity using tools such as ping and other network utilities

## What I Learned

This lab helped me better understand how firewall rules, routing, NAT, IP addressing, and network services work together.

It also reinforced the importance of troubleshooting networks layer by layer instead of changing multiple settings at once.

## Future Improvements

- Add a network diagram
- Add screenshots of the pfSense configuration
- Document specific firewall rules
- Demonstrate allowed vs. blocked traffic
- Add packet analysis with Wireshark
