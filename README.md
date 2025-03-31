# Windows-Metasploit-Kali-UTM-Setup
This project documents the setup of a virtual lab using UTM to run Windows 11, Kali Linux, and Metasploit for cybersecurity research and penetration testing. It includes step-by-step instructions for installation, configuration, and creating a secure, isolated environment for ethical hacking practice. 
## Windows 11, Metasploit & Kali Linux Setup on UTM

### Prerequisites
- UTM installed on macOS
- Windows 11 ISO
- Kali Linux ISO
- Metasploit Framework

---

## Step 1: Install UTM
1. Download UTM from [UTM Website](https://mac.getutm.app/).
2. Install UTM using the provided DMG file.
3. Launch UTM.

---

## Step 2: Set Up Windows 11
1. Create a new virtual machine (VM) in UTM.
2. Select **Windows** and upload the Windows 11 ISO.
3. Configure RAM, CPU, and storage as needed.
4. Install Windows 11 using the on-screen instructions.

---

## Step 3: Set Up Kali Linux
1. Create another VM for Kali Linux.
2. Choose **Linux** and upload the Kali Linux ISO.
3. Install using the default settings.
4. Update Kali Linux and install essential tools using:
    ```bash
    sudo apt update && sudo apt upgrade
    sudo apt install metasploit-framework
    ```

---

## Step 4: Install and Configure Metasploit
1. Start Kali Linux and open a terminal.
2. Run:
    ```bash
    msfconsole
    ```
3. Confirm Metasploit is running.

---

## Step 5: Network Configuration
- Set both VMs to **NAT** or **Bridged Network** mode for network connectivity.
- Ensure proper firewall rules are in place.

---

## Conclusion
You now have a working cybersecurity lab for penetration testing using Metasploit on Kali Linux. 
