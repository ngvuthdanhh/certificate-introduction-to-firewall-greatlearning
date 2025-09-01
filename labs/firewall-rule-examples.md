# Lab 2: Firewall Rule Examples

## Objective
Practice creating and applying firewall rules using different methods.

## Examples

### Example 1: Block a specific IP
```bash
sudo ufw deny from 192.168.1.100
```
Example 2: Allow traffic to a specific port

```bash
sudo ufw allow 443/tcp
```

Example 3: Limit SSH connections

```bash
sudo ufw limit ssh
```

Example 4: Check and delete rules

```bash
sudo ufw status numbered
sudo ufw delete <rule_number>
```

Expected Outcome

- Rules correctly block or allow traffic as configured.

- Confirm rule changes using sudo ufw status.

---
