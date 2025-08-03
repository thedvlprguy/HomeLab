# 🛡️ SOC Homelab on Windows 10

A beginner-friendly homelab designed to simulate a Security Operations Center (SOC) environment using a Windows 10 host. Perfect for those starting out in cybersecurity, IT support, or blue team roles.

## 🧰 Tools Used

* Windows 10 (Host OS)
* VirtualBox or VMware
* Parrot Security OS / Kali Linux (VM)
* ELK Stack (Optional)
* Sysmon + Windows Event Forwarding (Optional)

---

## 📦 Step-by-Step Setup

### 1. Install Virtualization Software

* Download and install [VirtualBox](https://www.virtualbox.org/) or [VMware Workstation Player](https://www.vmware.com/products/workstation-player.html).
* Enable virtualization in your BIOS if not already.

### 2. Create VMs

#### 🔹 Windows 10 VM

* Install a Windows 10 ISO in a VM.
* Enable RDP and create multiple local users to simulate an enterprise system.
* Install Sysmon (for advanced logging):
  [Download Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)

#### 🔹 Parrot Security / Kali Linux VM

* Install from ISO (available at [ParrotSec](https://www.parrotsec.org/) or [Kali Linux](https://www.kali.org/)).
* This will act as your SOC analyst system.
* Install tools like:

  * Wireshark
  * Zeek
  * Splunk Free / ELK Stack (optional)
  * Logstash and Filebeat (if collecting logs)

---

## 🔧 What You Can Practice

* Log analysis from the Windows VM
* Simulating and detecting brute force/RDP attacks
* Detecting privilege escalation attempts
* Using PowerShell logs and Sysmon to detect suspicious activities
* Configuring SIEM-like behavior with ELK/Splunk

---

## 📂 Folder Structure

```
SOC-Homelab/
├── VMs/
│   ├── Windows10/
│   └── ParrotSec/
├── Logs/
│   └── sysmon-logs/
├── Scripts/
│   └── incident-simulations.ps1
└── README.md
```

---

## ⚠️ Notes

* Always isolate your lab from your main network using NAT or Host-only adapter.
* This is a **learning environment** — do not use real malware or connect unprotected VMs to the internet.
* Use snapshots to revert after simulating attacks.

---

## 📎 Useful Resources

* [Malware Traffic Analysis Lab](https://www.malware-traffic-analysis.net/)
* [Hunting with Sysmon](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon)
* [Splunk Security Use Cases](https://lantern.splunk.com/)

---


