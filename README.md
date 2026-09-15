# 🔎 Nmap Network Reconnaissance Lab

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-blue)
![Nmap](https://img.shields.io/badge/Tool-Nmap-red)
![Kali Linux](https://img.shields.io/badge/Platform-Kali%20Linux-black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

Network Scanning & Host Discovery

*W02-P02 | ZENMAP | NETWORK RECONNAISSANCE*
---
Field                                             Detail
---
## 🔹 Assessment Overview

| **Field**              | **Details**                                |
| :--------------------- | :----------------------------------------- |
| 👨‍💻 **Pentester**    | **Kabo Sekoto**                            |
| 🎓 **Program / Batch** | **B0823 — Networkwalks**                    |
| 📅 **Date**            | **16 September 2026**                      |
| 🧪 **Module**          | **W2— Zenmap Scanning**               |
| 🎯 **Client / Target** | **Portswigger Network**                  |
| 🔐 **Authorization**   | ✅ **Permission Secured**                   |
| 🛰️ **Phase**          | **Phase 2 — Scanning and Network Discovery** |
| 📌 **Assessment Type** | **Authorized Network Reconnaissance**      |


## 1.⚠️ Liability Disclaimer

All activities were performed for educational purposes on authorized training environments, including PortSwigger Web Security Academy. No unauthorized systems or devices were targeted. All testing remained within permitted lab boundaries.

## 2. Introduction

This report covers network scanning, host discovery and information gathering using Zenmap and authorized Cybersecurity training environments. The objective was to identify hosts and collect basic information such as IP addresses, MAC addresses and hostnames.

*All activities were performed within authorized environments, including my local LAN and PortSwigger Web Security Academy.*

## 🛠️ 3. Tools Used

| **Tool**                  | **Purpose**                             |
| :------------------------ | :-------------------------------------- |
| 💻 **Windows CMD**        | Identify local network configuration    |
| 🛰️ **Zenmap (Nmap GUI)** | Discover live hosts and network devices |

---

## 🔍 4. Activities Performed

### 4.1 Network Identification

The local network configuration was first identified using **Windows CMD**. The identified subnet was then configured in **Zenmap** to perform authorized host discovery and identify active devices on the network.

**Command executed:**

```bash
nmap -sn 192.168.178.175/24
```

> **Scan Type:** Host Discovery (`-sn`)
> **Objective:** Identify live hosts on the target network.

Evidence:
![Network Configuration](screenshots/network-config.png)

### 4.2 Network Scanning with Zenmap

Zenmap Ping Scan identified **9 active hosts** across **256 IP addresses**.

| **#** | **IP Address**   | **Host / Device** |
| :---: | :--------------- | :---------------- |
|   01  | `192.168.178.1`  | Router            |
|   02  | `192.168.178.21` | Chantals-iPhone   |
|   03  | `192.168.178.22` | Ditalala-PC       |
|   04  | `192.168.178.23` | HP Device         |
|   05  | `192.168.178.49` | Hikvision Device  |

> **Result:** 9 hosts up / 256 IPs scanned

**📸 Evidence — Zenmap Scan**

![Zenmap Scan](evidence/zenmap-scan.png)


### 4.3 IP and MAC Address Discovery

Zenmap was used to identify **IP and MAC addresses** of discovered hosts, providing basic device identification information.

**📸 Evidence — IP & MAC Address Discovery**

![IP and MAC Addresses](screenshots/ip-mac-addresses.png)

### 4.4 Network Topology

Zenmap’s **Topology** feature was used to visualize the discovered network environment and connected hosts.

**📸 Evidence — Zenmap Network Topology**

![Zenmap Topology](screenshots/zenmap-topology.png)

## ⚠️ 5. Risk Analysis / Impact

| **#** | **Risk / Finding**        | **Observation**                  | **Potential Impact**                         |                 **Risk Level**                 |
| :---: | :------------------------ | :------------------------------- | :------------------------------------------- | :--------------------------------------------: |
|   01  | **Multiple live hosts**   | 9 active hosts discovered        | Unknown devices may be present               | <span style="color:orange">●</span> **Medium** |
|   02  | **IP addresses exposed**  | Internal IP addresses identified | Network structure may be mapped              |   <span style="color:green">●</span> **Low**   |
|   03  | **MAC addresses visible** | MAC information returned by Nmap | Connected hardware may be identified         |   <span style="color:green">●</span> **Low**   |
|   04  | **Hostnames exposed**     | Device names identified          | May reveal information about network devices |   <span style="color:green">●</span> **Low**   |

### 🔑 Risk Level Key

<span style="color:red">●</span> **High**    <span style="color:orange">●</span> **Medium**    <span style="color:green">●</span> **Low**

> **Note:** *These findings are observations from the network discovery exercise and **do not represent confirmed vulnerabilities***.

## 🛡️ 6. Recommendations

* Regularly scan the local network for **unknown or newly active devices**.
* Verify all **live hosts** and connected devices.
* Maintain an updated **device inventory**.
* Use strong **Wi-Fi security** and authentication.
* Monitor for **unusual or unauthorized network activity**.
* Perform security scanning only on **authorized systems and networks**.

## ✅ 7. Conclusion

During **Week 2** of my cybersecurity practical training, I used **Zenmap/Nmap** to perform network discovery on my local LAN. The scan identified **9 live hosts** and provided details such as IP addresses, MAC addresses, and hostnames.

This practical strengthened my understanding of **host discovery, network mapping, and the scanning phase** of an authorized security assessment.

## 8. Evidence Collected

### E01 — Network Configuration

**Evidence:** `network-config.png`

> **Screenshot:**
> *[Insert Network Configuration screenshot here]*

---

### E02 — Zenmap Scan Results

**Evidence:** `zenmap-scan.png`

> **Screenshot:**
> *[Insert Zenmap Scan screenshot here]*

---

### E03 — Discovered Hosts

**Evidence:** `discovered-hosts.png`

> **Screenshot:**
> *[Insert Discovered Hosts screenshot here]*

---

### E04 — IP & MAC Address Discovery

**Evidence:** `ip-mac-addresses.png`

> **Screenshot:**
> *[Insert IP & MAC screenshot here]*

---

### E05 — Network Topology

**Evidence:** `zenmap-topology.png`

> **Screenshot:**
> *[Insert Network Topology screenshot here]*



## 📊 Project Summary

| **Category**              | **Details**                       |
| :------------------------ | :-------------------------------- |
| **Project**               | Cybersecurity Lab — Week 02       |
| **Focus**                 | Network Scanning & Host Discovery |
| **Tool**                  | Zenmap / Nmap                     |
| **Target Network**        | `192.168.178.175/24`                |
| **Live Hosts Identified** | **9**                             |
| **Status**                | **Completed**                     |

## 👤 Author

### Kabo Sekoto
**🔐 Junior Cybersecurity Practitioner**

> `Learning → Building → Testing → Securing`

This repository forms part of my practical cybersecurity learning portfolio and documents my hands on laboratory exercises..

<p align="center">
  <a href="https://linkedin.com/in/kabosekoto">
    <img src="https://img.shields.io/badge/🔵_LinkedIn-Professional%20Profile-0A66C2?style=for-the-badge" />
  </a>
  &nbsp;
  <a href="https://www.youtube.com/@IamSkottK">
    <img src="https://img.shields.io/badge/🔴_YouTube-Cybersecurity%20Lab-FF0000?style=for-the-badge" />
  </a>
</p>


---
