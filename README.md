# Day-4 Internship
## Task 4: Setup and Use a Firewall on Linux (Using UFW)
### 1. Opened Terminal and Checked UFW Status
```bash
sudo ufw status verbose
```

### 2. Added a Rule to Block Port 23 (Telnet)
```bash
sudo ufw deny 23
```
- This blocked inbound connections on port 23.

---

### 3. Tested the Block Rule
```bash
telnet localhost 23
```
- The connection was refused, confirming the firewall was working as intended.

---


### 4. Removed the Block Rule to Restore Original State
```bash
sudo ufw delete deny 23
```
- Cleaned up the test rule.

---


### 5. Verified Firewall Rules for Deliverable
```bash
sudo ufw status numbered
```
- Took a screenshot of this output as required.

---

