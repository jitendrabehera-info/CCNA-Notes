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
<img width="515" height="534" alt="image" src="https://github.com/user-attachments/assets/d2da1d05-b518-47a4-9b25-76bc0fe10936" />

* Network Adapter → **NAT(Recommended)**

* <img width="1919" height="985" alt="image" src="https://github.com/user-attachments/assets/63408682-56b0-40fc-9f8c-d52d7466ee5c" />


✅ Enable:

* Virtualize Intel VT-x / AMD-V

  <img width="887" height="914" alt="image" src="https://github.com/user-attachments/assets/9d2031a9-c9a9-4946-8ebd-24cf708daf33" />


---

## 📀 Step 3: Attach ISO

* Go to **CD/DVD**
* Select **Use ISO Image**
* Attach your **EVE-NG ISO file**

* <img width="890" height="452" alt="image" src="https://github.com/user-attachments/assets/0e1eb144-3384-4ca9-82ac-3fd16abcfa27" />


---

## ▶️ Step 4: Install EVE-NG

1. Power ON the VM
2. Select: **Install EVE-NG Community Edition**
3. Follow installation steps:

   * Language → Select (English) Press enter
   * <img width="1332" height="560" alt="image" src="https://github.com/user-attachments/assets/57b39a09-7b72-4dc8-aeb0-aeafb9318cf3" />

   * Keyboard → Press Enter (Done)
  <img width="1407" height="817" alt="image" src="https://github.com/user-attachments/assets/dad12bb8-62f0-47f8-9c43-8ed333746254" />

   * Select Continue (Press Enter)
4. Wait for installation to complete
5. it's take Lot's Of time

---

## 🔐 Step 5: CLI Login

```
Username: root
Password: eve
```
-> root password (empaty - Press OK) -> Hostname (Default) -> Domain/system (Deault) -> DHCP -> direct connection (press enter) -> It's going to reboot
---

## 🌐 Step 6: Get IP Address

Example output:

```
192.168.1.100
```
<img width="548" height="77" alt="image" src="https://github.com/user-attachments/assets/8937f0dd-6bfc-4a0a-9867-a0014d5dd48b" />

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
(Select Native console)
<img width="1900" height="935" alt="image" src="https://github.com/user-attachments/assets/25156573-0e3e-4d0c-b40d-f69e36a48aca" />

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

## ✅ Done!

Your EVE-NG lab is now ready 🚀

---
