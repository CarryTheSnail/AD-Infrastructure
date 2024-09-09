<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This part of the project outlines the steps in building the infrastructure for deploying Active Directory on Azure. We will use one of the VMs created in this project as the Domain Controller and the other one as the client computer.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Create two VM on Azure.
    - Name the first VM, "DC-1" (Domain Controller) and the second, "Client-1" (User
    - Use "Windows Server 2022" for DC-1
    - Use "Windows 10 Pro" for Client-1
- Step 2: Set DC-1's IP Address to static
    - Network Settings -> Network Interface/IP configuration -> ipconfig1
- Step 3: Login to DC-1 with Remote Desktop Connection and disable Windows Firewall (for testing connectivity)
- Step 4: Set Clent-1's DNS settings to DC-1's Private IP Address (10.0.0.4)
- Step 5: Login to Client-1 in RDC. Attempt to ping DC-1's private Address 10.0.0.4.
    - Open PowerShell and run ipconfig/all. The output for the DNS settings should show DC-1's private IP Address.

<h2>Deployment and Configuration Steps</h2>

Step 1: Create two VM on Azure. Name the first VM, "DC-1" (Domain Controller) and the second, "Client-1" (User). Use "Windows Server 2022" for DC-1. Use "Windows 10 Pro" for Client-1
    
![image](https://github.com/user-attachments/assets/5a5e9faa-feda-4fb7-ad9e-fc51e1a46544)

<br />

Step 2: Set DC-1's IP Address to static. Network Settings -> Network Interface/IP configuration -> ipconfig1
![image](https://github.com/user-attachments/assets/22262e1d-ca0c-452e-8517-163b2dd59343)
![image](https://github.com/user-attachments/assets/10de253f-fcdf-4c3c-9f23-58c228f2d02c)

<br />

Step 3: Login to DC-1 with Remote Desktop Connection and disable Windows Firewall (for testing connectivity)

![image](https://github.com/user-attachments/assets/1a74289e-9b32-4eb9-8026-cfc03a97029f)

<br />

Step 4: Set Clent-1's DNS settings to DC-1's Private IP Address (10.0.0.4)

![image](https://github.com/user-attachments/assets/0cb74387-8f85-486b-89b2-262fcaeb409a)

<br />

Step 5: Login to Client-1 in RDC. Attempt to ping DC-1's private Address 10.0.0.4. Open PowerShell and run ipconfig/all. The output for the DNS settings should show DC-1's private IP Address.

![image](https://github.com/user-attachments/assets/f2e322f5-c3d6-49ef-aa62-00cf7a2c7258)
![image](https://github.com/user-attachments/assets/136059af-99ba-4a9c-8ea6-1067b6717af5)

<br />

