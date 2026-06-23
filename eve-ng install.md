# 🚀 EVE-NG Installation on VMware Workstation (Step-by-Step)
---

## 📌 Prerequisites

Make sure your system meets the following:

* 💻 VMware Workstation / VMware Player installed
* 📀 EVE-NG ISO file downloaded  (Free EVE Community Edition)
https://www.eve-ng.net/index.php/download/#DL-COMM
<img width="1741" height="870" alt="image" src="https://github.com/user-attachments/assets/95b4eca8-0fc1-4767-b950-1c82732999d4" />



* 🧠 Minimum Specs:

  * RAM: 8 GB (16 GB recommended)
  * CPU: 4 Cores
  * Disk: 100 GB
* ⚙️ Virtualization enabled in BIOS (Intel VT-x / AMD-V)

---

## 🛠️ Step 1: Create Virtual Machine

1. Open VMware Workstation
2. Click **Create New Virtual Machine**
3. Select **Typical (Recommended)**
4. Choose **I will install the OS later**
5. Select:

   * OS: `Linux`
   * Version: `Ubuntu 64-bit`
6. Name the VM: `EVE-NG`

---

## ⚙️ Step 2: Configure Hardware

Click **Customize Hardware** and set:

* RAM → 8 GB or higher
* CPU → 4 cores
* Hard Disk → 100 GB
* Network Adapter → **Bridged (Recommended)**

✅ Enable:

* Virtualize Intel VT-x / AMD-V

---

## 📀 Step 3: Attach ISO

* Go to **CD/DVD**
* Select **Use ISO Image**
* Attach your **EVE-NG ISO file**

---

## ▶️ Step 4: Install EVE-NG

1. Power ON the VM
2. Select: **Install EVE-NG Community Edition**
3. Follow installation steps:

   * Language → Select
   * Keyboard → Select
   * Disk → Automatic partition
4. Wait for installation to complete
5. Reboot VM

---

## 🔐 Step 5: CLI Login

```
Username: root
Password: eve
```

---

## 🌐 Step 6: Get IP Address

Run:

```
ip a
```

Example output:

```
192.168.1.100
```

---

## 🌍 Step 7: Access Web Interface

Open browser:

```
https://<EVE-IP>
```

Login:

```
Username: admin
Password: eve
```

---

## ❗ Troubleshooting

### 🔴 VM not starting

* Enable virtualization in BIOS
* Disable Hyper-V (Windows)

---

### 🔴 No IP address

* Change network to **Bridged Mode**

---

### 🔴 Web UI not opening

Run:

```
systemctl restart apache2
```

---

## 📂 Upload Network Images

Use tools like **WinSCP** and upload images to:

```
/opt/unetlab/addons/qemu/
```

---

## 💡 Pro Tips

* Install:

  * Cisco IOSv / IOU
  * Fortinet Firewall
  * Palo Alto VM
* Practice:

  * Routing & Switching
  * Firewall configs
  * Security labs

---

## 🎯 Use Cases

* CCNA / CCNP Lab Practice
* Cybersecurity Testing
* Network Simulation
* Real-world topology building

---

## ✅ Done!

Your EVE-NG lab is now ready 🚀

---
