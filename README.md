# cloud-cybersecurity-lab
# ☁️ Cloud Cybersecurity Lab (Azure + Kali Linux)

## 📌 Overview
This project demonstrates the deployment of a cloud-based penetration testing lab using Microsoft Azure and Kali Linux. The lab is used for practicing ethical hacking techniques, network reconnaissance, and vulnerability testing in a controlled environment.

---

## 🚀 Current Progress
✔ Kali Linux VM deployed on Azure  
✔ SSH remote access configured  
✔ Kali tools installed  
✔ OWASP Juice Shop deployed  
✔ Initial Nmap scans completed  

---

## 🔜 Next Steps
- Perform deeper Nmap scans (service + OS detection)
- Conduct web testing using Burp Suite
- Identify and document vulnerabilities
- Deploy additional vulnerable machines for testing

---

## 🛠️ Environment Setup

### 1. Connect to VM (SSH)
```bash
ssh -i "/path/to/your-key.pem" azureuser@<your-vm-ip>


### 2. Update System
```bash
sudo apt update && sudo apt upgrade -y

3. Install Kali Tools
sudo apt install -y kali-linux-default

4. Create Lab Directory
mkdir ~/lab
cd ~/lab
pwd

5. Verify Installation
nmap --version

6, Safe Scan Practice
nmap scanme.nmap.org

🖥️ GUI + Remote Desktop Setup
Install Desktop Environment
sudo apt install -y xfce4 xfce4-goodies

Install XRDP
sudo apt install -y xrdp
sudo systemctl enable xrdp
sudo systemctl start xrdp

Check XRDP Status
sudo systemctl status xrdp

Set User Password
sudo passwd azureuser

🌐 Azure Networking (RDP Access)

Configure inbound rule:

Port: 3389

Protocol: TCP

Action: Allow

💻 Connect via Remote Desktop

Press Windows + R

Type mstsc

Enter IP: <your-vm-ip>

Login with your credentials

🔍 Tools & Techniques Used

Nmap

Metasploit Framework

OWASP Juice Shop

Kali Linux

🧠 Key Skills Demonstrated

Cloud deployment using Azure

Linux system administration

Network scanning & reconnaissance

Remote access setup (SSH + RDP)

⚠️ Ethical Use Notice

All testing was done in a controlled lab. Do NOT scan networks without permission.
