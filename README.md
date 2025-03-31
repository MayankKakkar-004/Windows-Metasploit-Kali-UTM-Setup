# Windows-Metasploit-Kali-UTM-Setup

This project documents the setup of a virtual lab using UTM to run Windows 11, Kali Linux, and Metasploit for cybersecurity research and penetration testing. It includes step-by-step instructions for installation, configuration, and creating a secure, isolated environment for ethical hacking practice.

---

## Prerequisites
- **UTM** installed on macOS
- **Windows 11 ISO** - [Download Link](https://www.microsoft.com/en-us/software-download/windows11)
- **Kali Linux ISO** - [Download Link](https://www.kali.org/get-kali/)
- **Metasploit Framework** - [Download Link](https://www.metasploit.com/)

---

## Step 1: Install UTM
1. Download UTM from the [official website](https://mac.getutm.app/).
2. Install UTM using the provided `.dmg` file.
3. Launch UTM and ensure it opens successfully.

---

## Step 2: Set Up Windows 11
1. In UTM, click on **Create a New Virtual Machine**.
2. Select **Windows** as the operating system.
3. Upload the [Windows 11 ISO](https://www.microsoft.com/en-us/software-download/windows11).
4. Allocate RAM, CPU, and storage space as needed.
5. Follow the installation steps to install Windows 11.

---

## Step 3: Set Up Kali Linux
1. Create another virtual machine in UTM.
2. Choose **Linux** and upload the [Kali Linux ISO](https://www.kali.org/get-kali/).
3. Allocate appropriate resources (CPU, RAM, Disk Space).
4. Install Kali Linux using guided settings.
5. After installation, update your packages:
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```

---

## Step 4: Install Metasploit
1. Open Kali Linux.
2. Install Metasploit using the following command:
    ```bash
    sudo apt install metasploit-framework -y
    ```
3. Start Metasploit using:
    ```bash
    msfconsole
    ```
4. Verify it is working correctly.

---

## Step 5: Network Configuration
- Set both VMs to **NAT** or **Bridged Network** mode for connectivity.
- Ensure firewall rules allow communication between the VMs.

---

## Troubleshooting Tips
- If Kali Linux VM fails to start, check UTM logs and increase RAM or CPU allocation.
- If Metasploit crashes, ensure Kali Linux is updated:
    ```bash
    sudo apt update && sudo apt upgrade -y
    ```

---

## Conclusion
You now have a fully functional cybersecurity lab using UTM. This setup is perfect for practicing penetration testing, network analysis, and ethical hacking using Metasploit.

Feel free to contribute improvements or suggest additional configurations!

---

## Resources
- [UTM Documentation](https://docs.getutm.app/)
- [Kali Linux Documentation](https://www.kali.org/docs/)
- [Metasploit Guide](https://docs.metasploit.com/)


![Windows 11 iso Installation](/Users/mayankkakkar/Documents/win)


