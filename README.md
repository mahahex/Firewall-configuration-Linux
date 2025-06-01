# 🔥 Firewall Configuration – Windows & Linux 🧱

This project demonstrates how to configure and test basic firewall rules using **UFW** on Linux and **Windows Defender Firewall** on Windows. The goal is to control network traffic by allowing or blocking ports like a real-world cybersecurity analyst.

---

## 🎯 Objective

- Enable and use firewalls on Linux and Windows
- Block and allow traffic on specific ports
- Test connectivity using Telnet
- Understand how firewalls filter traffic
- Restore original configuration after testing

---

## 🧰 Tools Used

| Platform | Tool                         | Purpose                     |
|----------|------------------------------|-----------------------------|
| Linux    | UFW (Uncomplicated Firewall) | Firewall CLI                |
| Windows  | Windows Defender Firewall    | GUI-based firewall manager |
| Both     | Telnet                       | Test connectivity           |

---

## 🐧 Linux Setup: UFW Firewall

### 🔹 Commands Used

```bash
sudo ufw enable                  # Enable firewall
sudo ufw status verbose          # View current rules
sudo ufw deny 23                 # Block Telnet (port 23)
telnet localhost 23             # Test connection
sudo ufw allow 22                # Allow SSH (port 22)
sudo ufw delete deny 23         # Remove test block rule
