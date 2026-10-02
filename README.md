# Digital Forensics Lab — Operation Web Intrusion

An interactive, automated hands-on lab designed to teach the fundamentals of the **Digital Forensics Lifecycle** using **Autopsy**. 

This lab simulates a realistic corporate web server compromise where an attacker bypasses file upload security filters to upload a PHP backdoor, exfiltrates sensitive database tables, and executes anti-forensics scripts to wipe their tracks. Analysts must examine a virtual disk image to reconstruct the attack timeline, carve deleted files, identify extension signature mismatches, and identify the attacker's source IP.

---

## ⚙️ Quick Start Guide

To run this lab locally, you will need a **Kali Linux** virtual machine:

1.  **Clone or download** this repository onto your Kali Linux VM Desktop.
2.  Open your terminal, navigate to the directory, and make the setup script executable:
    ```bash
    chmod +x automate_lab.sh
    ```
3.  Execute the script with root privileges to build the virtual evidence disk:
    ```bash
    sudo ./automate_lab.sh
    ```
4.  The script will output `evidence.raw` on your **Desktop** along with its MD5 and SHA-256 integrity hashes.
5.  Launch Autopsy:
    ```bash
    sudo autopsy
    ```
6.  Open the web interface at `http://localhost:9999/autopsy`
