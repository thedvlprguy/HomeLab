# 🛠️ IT Support Homelab (Windows 10)

A simple homelab to practice IT Support tasks, including user management, troubleshooting, remote assistance, and system configuration — using only a Windows 10 setup and a few tools.

---

## 🧰 Tools Required

* **Windows 10 (Host or VM)**
* **VirtualBox or VMware** (if running additional VMs)
* **Sysinternals Suite**
* **Remote Desktop / AnyDesk**
* **Windows Admin Center** (optional)

---

## ⚙️ Lab Setup Steps

### 1. Create Virtual Machines (Optional)

* Use VirtualBox or VMware to create multiple Windows 10 VMs.
* Simulate a small office:

  * `User-PC`, `Admin-PC`, `Support-PC`.

### 2. Configure Users & Permissions

* Create multiple local users (Standard & Administrator roles).
* Practice:

  * Resetting passwords
  * Setting up UAC policies
  * Folder and printer sharing

### 3. Install Support Tools

* Download **Sysinternals Suite**:
  [https://learn.microsoft.com/en-us/sysinternals/downloads/](https://learn.microsoft.com/en-us/sysinternals/downloads/)
* Tools to explore:

  * `Process Explorer`
  * `Autoruns`
  * `PsExec`
  * `BGInfo`

### 4. Simulate Support Scenarios

* Fix network issues (IP config, DNS flush)
* Install/uninstall software
* Setup printers and shared drives
* Run system diagnostics (`sfc`, `DISM`)
* Use Event Viewer to check errors and logs

---

## 🧪 Practice Ideas

* Simulate a slow PC & troubleshoot it
* Setup and remove a local printer
* Troubleshoot broken internet on one VM
* Help a "user" install software using `PsExec`
* Use RDP/AnyDesk for remote troubleshooting

---

## 📁 Folder Structure

```
ITSupport-Homelab/
├── VMs/
│   ├── Admin-PC/
│   └── User-PC/
├── Tools/
│   └── Sysinternals/
├── Scripts/
│   └── fix-network.ps1
└── README.md
```

---

## ⚠️ Tips

* Keep snapshots of your VM to revert after testing.
* Avoid connecting lab VMs to your main network.
* Use NAT or host-only networking.

---

## 📎 Resources

* [Windows Troubleshooting Guide](https://support.microsoft.com/en-us/windows)
* [Microsoft Learn - Windows Admin Skills](https://learn.microsoft.com/en-us/training/windows/)
* [Sysinternals Documentation](https://learn.microsoft.com/en-us/sysinternals/)

---
