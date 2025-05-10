## 📁 Remote Imaging of a System using FTK Imager

### 📝 Overview

This project sets up an **agent-based remote imaging environment** using **FTK Imager**, enabling digital forensic investigators to perform remote disk imaging of suspect machines efficiently and securely. The captured disk images can be saved to a central file server and analyzed using forensic tools like **Autopsy**.


### ![icons8-tools-24](https://github.com/user-attachments/assets/c5098d8c-f991-4d8e-944f-28b8cbdabd25) Tools Used

- **FTK Imager** – Disk imaging tool.
- **Autopsy** – Open-source digital forensic platform.
- **Remote Access Protocols** – RDP, SSH, etc.
- **Shared Fileserver** – Centralized secure storage.


### 🧩 Components/Tools Involved

1. **Workstation** Digital Forensic Investigator Workstation
2. **Remote Suspect Machines** - Laptops/Desktops
3. **FTK Imager** - Installed as an Imaging tool, alternative to Encase Agent
4. **Shared Fileserver** - Central Storage
5. **Autopsy** - Forensic Analysis Tool
6. **Remote Access Protocols** - Remote Desktop Protocol (RDP)


### 🔁 Workflow Description

1. **Investigator Initialization**:  
   The process starts with the Digital Forensic Investigator establishing remote access to the suspect machine(s).

2. **Remote Access**:  
   Secure remote connection is made to the target machines using RDP, or any remote management solution.

3. **Target Machine Access**:
   The investigator connects to each remote system to be imaged.

4. **FTK Imager Installation**:  
   FTK Imager is installed on the remote suspect machine, either manually or using deployment tools.

5. **Image Acquisition**:  
   Using FTK Imager, a disk image (logical or physical) of the target system is created.

6. **Image Storage**:  
   The image is saved to a **Shared Fileserver** (network attached storage) to avoid using local suspect system resources.

7. **Remote Image Availability**:  
   The image is stored and made accessible over the network for further analysis.

8. **Case Creation & Analysis**:  
   The investigator uses **Autopsy** to create a case and analyze the image, performing forensic analysis remotely without physical access to the suspect machine.

![DF_RemoteImaging drawio](https://github.com/user-attachments/assets/151edebc-cc33-434b-bd38-17e3141deca6)


### 🛠 Setup Instructions

1. **Install FTK Imager** on the target remote system.
2. **Map or provide access to a Shared Fileserver** to store the image files.
3. **Ensure Remote Access Tools** (e.g., RDP, SSH) are configured securely.
4. **Autopsy Setup** should be available on the forensic workstation.


### 🔒 Security Considerations

- Ensure all remote access is done over encrypted and authenticated channels.
- Use VPN or IP whitelisting to restrict access to imaging infrastructure.
- FTK Imager logs should be reviewed for completeness and integrity of image.

### 📌 Notes

- Avoid writing images to the same machine being imaged.
- Ensure time synchronization between systems for accurate timestamps.
- Maintain chain of custody documentation for legal admissibility.

### ![icons8-team-24](https://github.com/user-attachments/assets/6a585b1f-1313-4e0f-9808-74a87b99755f) Team Members
- [Shahzaib](https://github.com/Shahzaibali003)
- [Riazuddin Ahmed](https://github.com/riazuddinse)

