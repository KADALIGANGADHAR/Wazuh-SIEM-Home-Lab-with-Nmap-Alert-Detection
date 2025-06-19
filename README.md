# Wazuh-SIEM-Home-Lab-with-Nmap-Alert-Detection  

## Objective

### This project demonstrates the set up a Wazuh Security Information and Event Management (SIEM) system with a working agent and demonstrate alert generation and monitoring.

## Tools Used
- **Wazuh (Server & Dashboard)**
 
- **Ubuntu (Wazuh server VM)**
 
- **Kali Linux (Agent system in VM)**
 
- **VMware**
 
- **Nmap (for triggering alerts)**
 
- **Elasticsearch, Kibana (comes with Wazuh)**
  
## ⚙️ Lab Setup

### 1.Installed Prerequisite Packages
#### ```sudo apt install curl``` 
#### ```sudo apt install default-jdk```
![Ubuntu 64-bit-2025-06-06-22-03-51](https://github.com/user-attachments/assets/310730c5-055e-410f-a90d-6aae3cba7869)
![Ubuntu 64-bit-2025-06-06-22-04-17](https://github.com/user-attachments/assets/851f39fa-eae8-45ab-973e-6ce2a6768128)
![Ubuntu 64-bit-2025-06-06-22-04-26](https://github.com/user-attachments/assets/63710ee7-991c-4d84-9c6f-af0df4f9a90d)
![Ubuntu 64-bit-2025-06-06-22-04-30](https://github.com/user-attachments/assets/d261d876-c811-402c-a713-f15b2382b841)
![Ubuntu 64-bit-2025-06-06-22-04-34](https://github.com/user-attachments/assets/1136bb4e-efdc-4dfc-b40f-915e1985b85a)
### 2.Installed Wazuh Using Official Script
#### Downloaded and executed the ocial Wazuh installation script to set up the Wazuh server,dashboard, and components.dashboard, and components.
![Ubuntu 64-bit-2025-06-06-22-05-04](https://github.com/user-attachments/assets/ce61b60f-1a6c-4104-80ce-83a98eefff32)
#### ```curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh```
![Ubuntu 64-bit-2025-06-06-22-05-10](https://github.com/user-attachments/assets/d92f362a-8d69-4007-8f32-dc18c631a21c)
![Ubuntu 64-bit-2025-06-06-22-09-37](https://github.com/user-attachments/assets/eb6a3118-45be-45db-9312-171d6bb2a18f)
![Ubuntu 64-bit-2025-06-06-22-22-38](https://github.com/user-attachments/assets/ab2435b1-5fb6-4df8-8cf2-be971587d2a4)
![Ubuntu 64-bit-2025-06-06-22-22-43](https://github.com/user-attachments/assets/fff35b46-e88b-413d-a87b-b8d3039cba9d)
![Ubuntu 64-bit-2025-06-06-22-23-46](https://github.com/user-attachments/assets/db30794f-b59c-4186-9619-b1b79f853530)



