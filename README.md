
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
##Images for refernce 
##Windows 
<img width="889" alt="Screenshot 2025-03-31 at 9 00 39 PM" src="https://github.com/user-attachments/assets/ab7932d4-b980-4a41-bb73-151ea22f382a" />
<img width="650" alt="Screenshot 2025-03-31 at 9 02 56 PM" src="https://github.com/user-attachments/assets/b1dabd0e-1f82-4a05-b39a-bcac38bf8f71" />
<img width="998" alt="Screenshot 2025-03-31 at 9 02 01 PM" src="https://github.com/user-attachments/assets/35a2e4a7-c48d-4a03-8e90-391a5b0cfe41" />
<img width="1036" alt="Screenshot 2025-03-31 at 9 01 56 PM" src="https://github.com/user-attachments/assets/eae3f99d-d417-4374-8690-fc1632cf9f60" />
<img width="1288" alt="Screenshot 2025-03-31 at 9 01 37 PM" src="https://github.com/user-attachments/assets/d659aea0-8b1b-42a8-8edb-a19a632566ce" />
<img width="820" alt="Screenshot 2025-03-31 at 9 01 29 PM" src="https://github.com/user-attachments/assets/f40b2070-7c89-469d-813f-e367419cf343" />
<img width="827" alt="Screenshot 2025-03-31 at 9 01 21 PM" src="https://github.com/user-attachments/assets/5e1efc37-6241-4089-b76d-1c059dc5a0a6" />
<img width="772" alt="Screenshot 2025-03-31 at 9 00 59 PM" src="https://github.com/user-attachments/assets/caab91b7-a760-4bb5-9fc2-90a1b908f53c" />
<img width="919" alt="Screenshot 2025-03-31 at 9 00 54 PM" src="https://github.com/user-attachments/assets/4c9bbd7d-7698-470b-9d90-bb042563c16f" />
<img width="704" alt="Screenshot 2025-03-31 at 9 00 45 PM" src="https://github.com/user-attachments/assets/d164d9ae-dd6d-4c86-a447-aab403753f91" />

##Metasploit
<img width="877" alt="Screenshot 2025-03-31 at 9 10 02 PM" src="https://github.com/user-attachments/assets/d797ab3b-8753-4d82-ba62-24c0e9b5e43f" />
<img width="898" alt="Screenshot 2025-03-31 at 9 09 50 PM" src="https://github.com/user-attachments/assets/371e37ba-c1e9-4efc-b105-da9ba8d8aa44" />
<img width="744" alt="Screenshot 2025-03-31 at 9 09 30 PM" src="https://github.com/user-attachments/assets/c92ac4f9-f82b-4ce3-84a9-a989ae541f0c" />
<img width="913" alt="Screenshot 2025-03-31 at 9 09 20 PM" src="https://github.com/user-attachments/assets/61b43dbb-e8b6-492a-9862-47ee562320dd" />
<img width="736" alt="Screenshot 2025-03-31 at 9 08 55 PM" src="https://github.com/user-attachments/assets/724c6c84-1be7-4582-82b7-5fe79dea0eaf" />
<img width="741" alt="Screenshot 2025-03-31 at 9 08 39 PM" src="https://github.com/user-attachments/assets/90eaf144-e6eb-4765-bd78-239e9e93aefd" />
<img width="781" alt="Screenshot 2025-03-31 at 9 08 24 PM" src="https://github.com/user-attachments/assets/176eae11-9843-4ed1-9a14-2c82dd616566" />
<img width="773" alt="Screenshot 2025-03-31 at 9 08 18 PM" src="https://github.com/user-attachments/assets/4548d658-de6b-4e57-9379-a3ceb5387959" />
<img width="715" alt="Screenshot 2025-03-31 at 9 08 07 PM" src="https://github.com/user-attachments/assets/b637cba8-a16a-431a-8b6e-2edba089c359" />
<img width="777" alt="Screenshot 2025-03-31 at 9 08 02 PM" src="https://github.com/user-attachments/assets/5782fd1a-9f66-4891-8b9d-0ec6d9bbfe23" />
<img width="784" alt="Screenshot 2025-03-31 at 9 07 47 PM" src="https://github.com/user-attachments/assets/38de4fb0-f79f-407f-81d2-a60ba8ba9686" />
<img width="796" alt="Screenshot 2025-03-31 at 9 07 23 PM" src="https://github.com/user-attachments/assets/69959515-e901-4806-b308-fd4c07f90031" />
<img width="793" alt="Screenshot 2025-03-31 at 9 07 14 PM" src="https://github.com/user-attachments/assets/25fa500b-459f-4734-a6ea-dd466b1e4668" />
<img width="792" alt="Screenshot 2025-03-31 at 9 07 01 PM" src="https://github.com/user-attachments/assets/82216f33-e05b-40f3-b6d6-7334e673d4e0" />
<img width="1125" alt="Screenshot 2025-03-31 at 9 06 41 PM" src="https://github.com/user-attachments/assets/f65b3223-e93d-4bbc-ac5b-a640fe350c44" />
<img width="1149" alt="Screenshot 2025-03-31 at 9 06 34 PM" src="https://github.com/user-attachments/assets/92921823-420f-4c02-b71a-0dcdee359f2f" />


