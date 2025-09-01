# Firewall Commands Cheat Sheet

## UFW (Ubuntu)
- Enable firewall: `sudo ufw enable`
- Status: `sudo ufw status verbose`
- Allow port: `sudo ufw allow 80/tcp`
- Deny IP: `sudo ufw deny from 192.168.1.10`
- Delete rule: `sudo ufw delete <rule_number>`

## iptables (Linux)
- List rules: `sudo iptables -L -v -n`
- Allow port: `sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT`
- Block IP: `sudo iptables -A INPUT -s 192.168.1.10 -j DROP`
- Save rules: `sudo iptables-save > /etc/iptables/rules.v4`

## pfSense (Web GUI)
- Navigate: Firewall → Rules
- Add rule: Click "Add", choose interface, protocol, source, destination, action
- Apply changes: Click "Apply Changes" after editing
