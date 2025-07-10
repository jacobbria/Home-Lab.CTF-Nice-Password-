<h1 align="center">🖥️ Set-up for Devices and Systems</h1>

---

### 🎯 **Target System**

- 🖥️ **OS:** Windows Server 2022  
- ☁️ **Hosted On:** Azure Virtual Machine

---

### 🧨 **Attacker System**

- 🐾 **OS:** Kali Linux  
- 📦 **Hosted On:** VirtualBox VM

---

### 👤 **Account Details**

**Target (Windows Server):**
- Username: `Administrator`
- Initial Password: `Password123`
- Remote Access: RDP (enabled), SSH (enabled via optional features)

**Attacker (Kali):**
- Username: `kali`
- SSH Keys: Custom keypair generated for persistence testing

---

### 🛡️ **Target Security Configuration**

- 🔒 **Account Lockout Policy:**  
  10 failed login attempts allowed within 10 minutes before lockout  
- 🔐 **Remote Access:**  
  - RDP: Enabled (default Azure config)  
  - SSH: Enabled via Windows Optional Features  
- 🧱 **Firewall:**  
  Default Windows Defender Firewall rules active  
- 🛡 **AV/EDR:**  
  Windows Defender running (no third-party antivirus or EDR)

---

### 🧰 **Tools Installed (Attacker VM)**

- 🔍 **Recon & Enumeration**
  - `nmap`
  - `whois`
  - `nslookup`
- 🔐 **Brute Force & Auth Testing**
  - `hydra`
  - `medusa` (optional fallback)
- 📡 **Transfer & Exfil**
  - `scp`
  - `netcat`
  - `curl`
- 🕷️ **Other**
  - `Burp Suite`
  - `Wireshark`
  - `Metasploit Framework`

---

