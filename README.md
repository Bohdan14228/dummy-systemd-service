# dummy-systemd-service

Project: [https://roadmap.sh/projects/dummy-systemd-service](https://roadmap.sh/projects/dummy-systemd-service)  

🧠 Systemd Dummy Service
📋 Overview

This project demonstrates how to create and manage a custom systemd service in Linux.
The dummy service runs a background script that writes log messages every 10 seconds and restarts automatically if it fails.

⚙️ Setup
1️⃣ Create the script
```bash
sudo chmod +x /usr/local/bin/dummy.sh
```

2️⃣ Create the service file
```bash
sudo nano /etc/systemd/system/dummy.service

sudo systemctl daemon-reload
```

🧩 Usage
```bash
sudo systemctl start dummy
sudo systemctl stop dummy
sudo systemctl enable dummy
sudo systemctl disable dummy
sudo systemctl status dummy

sudo journalctl -u dummy -f
```

Remove
```bash
sudo systemctl stop dummy
sudo systemctl disable dummy
sudo rm /etc/systemd/system/dummy.service
sudo rm /usr/local/bin/dummy.sh
sudo systemctl daemon-reload
```
