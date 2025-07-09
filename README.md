# -Personal-Virtualized-Networking-and-Security-Lab
This project documents the deployment of a personal, virtualized networking and security lab environment for hands-on practice with enterprise-grade tools and services. The lab leverages Proxmox VE to virtualize network infrastructure, security appliances, and service hosts, simulating complex, real-world IT environments.

📦 Personal Virtualized Networking and Security Lab
Author: Modou Cham
Year: 2024
Status: In Progress / Complete (update as needed)

📖 Overview
This project documents the deployment of a personal, virtualized networking and security lab environment for hands-on practice with enterprise-grade tools and services. The lab leverages Proxmox VE to virtualize network infrastructure, security appliances, and service hosts, simulating complex, real-world IT environments.

🖥️ Lab Infrastructure
Device	Role
Lenovo Mini PC	Proxmox VE Hypervisor
Intel i5 Laptop	Client / Remote Management
Intel i3 Laptop	Additional VM Host / Testing

🛠️ Services & Tools Deployed
Proxmox VE — Virtualization platform

pfSense — Firewall & VPN

Active Directory (Windows Server / Samba) — Directory Services

Kali Linux — Penetration Testing

Docker Containers — Web apps & Services

OpenVAS — Vulnerability Scanning

Wireshark — Packet Analysis

RSAT — Remote Server Administration Tools

📑 Installation & Configuration Guides
📌 Proxmox VE Installation
Installed Proxmox VE on Lenovo Mini PC

Configured local storage and bridged networking

📌 pfSense Setup
Created pfSense VM in Proxmox

Configured WAN/LAN interfaces, firewall rules, DHCP, and VPN tunnels

📌 Active Directory Deployment
Installed Windows Server 2022 VM

Configured AD DS, DNS, DHCP, and Group Policies

Installed RSAT on management laptops

📌 Kali Linux Setup
Deployed Kali Linux VM

Installed penetration testing tools and configured network interfaces

📌 Docker Deployment
Installed Docker Engine on Ubuntu VM

Deployed web applications in isolated Docker containers

📌 OpenVAS Installation
Installed OpenVAS on a dedicated Ubuntu VM

Configured scanning policies and asset groups

🧪 Network Topology
Virtual networks, VLANs, and NAT configurations

Simulated multiple subnets and VPN tunnels for remote access

Monitored inter-VM traffic using Wireshark

🛡️ Security Testing & Monitoring
Conducted vulnerability scans with OpenVAS

Performed penetration testing simulations using Kali Linux

Monitored network traffic for analysis and troubleshooting

📓 Troubleshooting Notes
Resolved Proxmox networking issues by adjusting bridge configurations

Addressed pfSense DHCP conflicts and VPN tunnel instability

Fixed AD DNS resolution errors with forwarder and zone adjustments

Mitigated Docker container IP conflicts via custom bridge networks

📚 References
Proxmox Documentation

pfSense Docs

Active Directory Deployment Guide

Kali Linux Docs

Docker Docs

OpenVAS User Manual

📌 Future Improvements
Integrate SIEM solution (e.g. Wazuh, Graylog)

Automate VM deployments with Ansible

Configure HAProxy load balancer for Dockerized services

Document VPN performance benchmarks

