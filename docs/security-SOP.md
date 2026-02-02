# Operational Security & Data Integrity SOP

## 🚨 Data Safety Guardrail (Node 3)
**Requirement:** The 4TB Media Library is manually managed via `/etc/fstab`.
* **CRITICAL:** Never use the Proxmox GUI "Initialize Disk" function on the Media Node.
* **Reasoning:** Manual mounting with specific `uid=1000` ensures Docker container permission alignment.

## 🔐 Identity & Access Management (IAM)
* **Monitoring:** Use dedicated API Tokens (e.g., `PVEAuditor` role) for dashboards.
* **Principle:** Read-only access prevents accidental configuration changes through monitoring tools.

## 🌐 Network Hardening
* **Hardline DNS:** Router WAN settings are locked to the Pi-hole IP. No ISP fallback allowed.
* **VPN Routing:** All P2P traffic is encapsulated within a WireGuard tunnel.