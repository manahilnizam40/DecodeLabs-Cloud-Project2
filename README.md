# DecodeLabs-Cloud-Project2
# DecodeLabs Cloud Computing — Project 2: The Server Commander

## 📌 Project Overview
This repository contains the implementation for Project 2 of the DecodeLabs Cloud Computing Internship. The mission focuses on provisioning an AWS EC2 virtual machine, securing the environment with SSH keys and security groups, and deploying a custom Nginx web server hosting a welcome page.

---

## 🛠️ Mission Architecture & Tools
* **Cloud Provider:** Amazon Web Services (AWS EC2)
* **Operating System:** Amazon Linux 2023
* **Web Server Daemon:** Nginx
* **Authentication:** SSH Key Pair (.pem)
* **Firewall:** Security Groups (Port 22 for SSH, Port 80 for HTTP)

---

## 🚀 Execution Steps & Commands

Bash
ssh -i keyname.pem ec2-user@<Public-IP>

Bash
sudo dnf update -y
sudo dnf install nginx -y
sudo systemctl start nginx

HTML
<html>
<head>
<title>Fab and DecodeLabs</title>
</head>
<body>
<h1>Welcome to DecodeLabs: Mission Accomplished</h1>
</body>
</html>

 ### ScreenShots
 ![EC2 Instance Provisioning](./screenshot1.png)
 ![Security Groups Configuration](./screenshot2.png)

### 1. Secure Your Private Key (macOS / Linux)
```bash
chmod 400 keyname.pem
### ScreenShots
