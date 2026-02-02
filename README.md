# 🔱 Project Triumvirate: Federated Proxmox Homelab

## Executive Summary
Project Triumvirate is a high-availability, three-node Proxmox VE cluster designed for media automation, network monitoring (NOC), and security research. This repository documents an "On-Premise First" infrastructure strategy, emphasizing defense-in-depth, container orchestration, and automated service discovery.

**Targeting Certifications:** CompTIA Network+, Security+, Linux+, and WGU Network Engineering curriculum.

## 🏗️ Physical Infrastructure
| Node | Role | Hardware | Primary Services |
| :--- | :--- | :--- | :--- |
| **Node 1** | **The Brain** | ASUS Pentium N4200 | Cluster Master, NOC Dashboard, Uptime Kuma |
| **Node 2** | **The Shield** | Dell i3-4130T | Failover, Pi-hole (DNS), UniFi Controller |
| **Node 3** | **The Beast** | Lenovo G4560T | Docker Swarm/Compose, Media Pipeline, NetBox IPAM |

## 🛠️ Tech Stack & Skills Mapping
* **Virtualization:** Proxmox VE 8.x (Hypervisor management, LXC vs VM optimization).
* **Orchestration:** Docker Compose & Portainer (Container lifecycle management).
* **Networking:** WireGuard VPN Tunneling, DHCP/Static IP management via NetBox.
* **Security:** RBAC (Role-Based Access Control) via Proxmox API tokens.

## 🎓 Career Alignment (WGU/Professional)
* **Network+:** Implementation of Layer 3 IPAM and hardline DNS strategies.
* **Security+:** Application of the "Principle of Least Privilege" using PVEAuditor roles.
* **Linux+:** Manual filesystem mounting (`/etc/fstab`), permission management (UID 1000), and CLI troubleshooting.