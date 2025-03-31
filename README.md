
# Windows-Metasploit-Kali-UTM-Setup

This project documents the setup of a virtual lab using UTM to run Windows 11, Kali Linux, and Metasploit for cybersecurity research and penetration testing. It includes step-by-step instructions for installation, configuration, and creating a secure, isolated environment for ethical hacking practice.

---

## Prerequisites
- **UTM** installed on macOS
- **Windows 11 ISO**
- **Kali Linux ISO**
- **Metasploit Framework**

---

## Step 1: Install UTM
1. Download UTM from the [official website](https://mac.getutm.app/).
2. Install UTM using the provided `.dmg` file.
3. Launch UTM and ensure it opens successfully.

---

## Step 2: Download and Set Up Windows 11 ISO

Follow the steps below to download the Windows 11 ISO:

1. Visit the official [Windows 11 download page](https://www.microsoft.com/en-us/software-download/windows11).
2. Scroll down and under **"Create Windows 11 Installation Media"**, click on **Download now**.
3. This will download the **MediaCreationTool**. Open the tool after downloading.
4. Select **Create installation media (USB flash drive, DVD, or ISO file)** and click **Next**.
5. Choose **ISO file** and click **Next**.
6. Select the location where you want to save the ISO file and start the download process.
7. Once the download is complete, you’ll have the Windows 11 ISO file.

---

## Step 3: Download and Set Up Kali Linux ISO

Follow the steps below to download the Kali Linux ISO:

1. Visit the official [Kali Linux download page](https://www.kali.org/get-kali/).
2. Scroll down and you’ll find the **"Kali Linux ISO"** section.
3. Under **"Installer Images"**, select the appropriate image based on your system architecture (for most users, the **64-bit** version will be suitable).
4. Choose the **Installer** or **Live** version, depending on your preference (Installer allows for installation, Live runs directly without installation).
5. Click on the selected version and the download will begin.
6. After the download is complete, you’ll have the Kali Linux ISO file.

---

## Step 4: Download and Set Up Metasploit Framework

Metasploit is included in Kali Linux by default, but you can install it manually if needed. Here's how:

### **Download Metasploit**
1. Visit the official [Metasploit download page](https://www.metasploit.com/).
2. Scroll down and click on the **Download** button.
3. This will direct you to the **"Metasploit Community"** download page.
4. Choose the appropriate platform (Linux, Windows, or macOS) and follow the installation steps.

### **Install Metasploit on Kali Linux (if not already installed)**
1. Open the terminal on your Kali Linux VM.
2. Run the following command to install Metasploit Framework:
   ```bash
   sudo apt update && sudo apt install metasploit-framework -y
   ```
3. Once installation is complete, start Metasploit using the following command:
   ```bash
   msfconsole
   ```

---

## Step 5: Network Configuration
1. Set both the **Windows 11** and **Kali Linux** VMs in UTM to **NAT** or **Bridged Network** mode for proper networking and internet access.
2. Ensure firewall rules on both VMs are configured to allow communication between them.
3. Verify network connectivity using the **ping** command between the VMs to confirm they can communicate with each other.

---

## Troubleshooting Tips
- **Kali Linux VM fails to start**: If Kali Linux doesn’t start, check UTM logs and increase the allocated RAM or CPU resources.
- **Metasploit crashes**: Ensure that Kali Linux is updated by running:
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

---

## License
This project is licensed under the [MIT License](LICENSE).
