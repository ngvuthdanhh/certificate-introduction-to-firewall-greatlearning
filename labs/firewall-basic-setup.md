# Lab 1: Basic Firewall Setup

## Objective
Set up a basic firewall on a virtual machine or network device to control incoming and outgoing traffic.

## Requirements
- Virtual machine (Windows/Linux) or physical device
- Firewall software (e.g., iptables, pfSense, UFW)

## Steps
1. Install firewall software (if not built-in).
2. Verify current firewall status:

```bash
sudo ufw status
```

## Enable firewall:

```bash
sudo ufw enable
```

## Allow essential services (e.g., SSH, HTTP):

```bash
sudo ufw allow ssh
sudo ufw allow http
```

- Deny all other incoming connections by default.

- Test firewall rules by attempting connections from another device.

## Expected Outcome

- Only allowed services are accessible.

- Firewall blocks unauthorized connections.


---
