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
#### Downloaded and executed the official Wazuh installation script to set up the Wazuh server,dashboard, and components.dashboard, and components.
![Ubuntu 64-bit-2025-06-06-22-05-04](https://github.com/user-attachments/assets/ce61b60f-1a6c-4104-80ce-83a98eefff32)
#### ```curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh```
![Ubuntu 64-bit-2025-06-06-22-05-10](https://github.com/user-attachments/assets/d92f362a-8d69-4007-8f32-dc18c631a21c)
![Ubuntu 64-bit-2025-06-06-22-09-37](https://github.com/user-attachments/assets/eb6a3118-45be-45db-9312-171d6bb2a18f)
![Ubuntu 64-bit-2025-06-06-22-22-38](https://github.com/user-attachments/assets/ab2435b1-5fb6-4df8-8cf2-be971587d2a4)
![Ubuntu 64-bit-2025-06-06-22-22-43](https://github.com/user-attachments/assets/fff35b46-e88b-413d-a87b-b8d3039cba9d)
![Ubuntu 64-bit-2025-06-06-22-23-46](https://github.com/user-attachments/assets/db30794f-b59c-4186-9619-b1b79f853530)
### 3.Logged into Wazuh Dashboard
#### Accessed the Wazuh dashboard at https://192.168.235.140 using the default credentials:
![Ubuntu 64-bit-2025-06-06-22-24-37](https://github.com/user-attachments/assets/b8d2702b-e36b-44ed-a11e-b1b86e93b445)
![Ubuntu 64-bit-2025-06-06-22-24-41](https://github.com/user-attachments/assets/43d47594-5c27-4ea0-9271-c320b4776717)
![Ubuntu 64-bit-2025-06-06-22-25-23](https://github.com/user-attachments/assets/309bdc0e-c3ca-4ca7-8485-a2969839c0fc)
![Ubuntu 64-bit-2025-06-06-22-26-03](https://github.com/user-attachments/assets/ef0cc65a-f1da-4443-b704-7258282f965d)
#### Clicked on Deploy new agent
![Ubuntu 64-bit-2025-06-06-22-26-21](https://github.com/user-attachments/assets/d434422f-6c40-4495-aa06-37cd5e190b8b)
### 4.Configured and installed Wazuh agent on Kali Linux
![Ubuntu 64-bit-2025-06-06-22-27-13](https://github.com/user-attachments/assets/b0dafe6c-a922-47df-8acf-3b1565d95979)
![Ubuntu 64-bit-2025-06-06-22-27-57](https://github.com/user-attachments/assets/4eb20c4b-42dd-4b67-bdef-9d66c9b989b2)
![Ubuntu 64-bit-2025-06-06-22-28-07](https://github.com/user-attachments/assets/a4eb5fa8-8cfd-4fa3-8b9d-d2a1714c81aa)
### 5.Connected and Monitored Wazuh Agent
#### Verified that the agent (Ubuntu) was connected with ID 001, showing status as active.
![kali-linux-2024 4-vmware-amd64-2025-06-06-22-36-22](https://github.com/user-attachments/assets/54281579-5348-4807-9cd7-180a05bd2a6d)
![kali-linux-2024 4-vmware-amd64-2025-06-06-22-39-24](https://github.com/user-attachments/assets/7de18ac3-7ec4-4a02-aaef-8e504ee531c3)
### 6.Connected the agent to Wazuh server
![Ubuntu 64-bit-2025-06-06-22-39-57](https://github.com/user-attachments/assets/ef82c06d-0a56-4229-88af-9464dcb6928c)
### 7.Verified agent connection in dashboard
![Ubuntu 64-bit-2025-06-06-22-40-12](https://github.com/user-attachments/assets/5d80958a-fa0f-4a87-8d7f-dd61bacc2849)
### 8. Ran Nmap scans from Kali to generate alerts
 - **Basic Ping Scan (-sn)**
 - **TCP SYN Scan (-sS)**
 -  **Service Version Detection (-sV)**
 - **Aggressive Scan (-A)**
![kali-linux-2024 4-vmware-amd64-2025-06-07-12-36-33](https://github.com/user-attachments/assets/9f1c7f4a-1308-4420-94e6-5cb5c8548e9a)
![kali-linux-2024 4-vmware-amd64-2025-06-07-12-36-50](https://github.com/user-attachments/assets/87b0e78c-6f8c-4679-86cc-fe28a20f8651)
![kali-linux-2024 4-vmware-amd64-2025-06-07-12-36-57](https://github.com/user-attachments/assets/2bbcad06-91c0-4e4d-9585-aa3ad414a40f)
![kali-linux-2024 4-vmware-amd64-2025-06-07-12-37-03](https://github.com/user-attachments/assets/60847384-5578-41bc-b0e7-59ac39185ed7)
![kali-linux-2024 4-vmware-amd64-2025-06-07-12-37-10](https://github.com/user-attachments/assets/fbb769a2-e272-4605-a26d-8c32463f23e1)
### 9.Viewe logs in Wazuh Discover (wazuh-alerts-*)
![Ubuntu 64-bit-2025-06-06-22-45-26](https://github.com/user-attachments/assets/da65480f-266e-43c0-ac0e-024e5657b37f)
![Ubuntu 64-bit-2025-06-06-22-46-21](https://github.com/user-attachments/assets/fbb768b5-5aee-47d4-ae66-9eee7c5ac3eb)
![Ubuntu 64-bit-2025-06-06-22-50-53](https://github.com/user-attachments/assets/c15d2614-eb48-4945-aad9-49fda85c6ce6)
![Ubuntu 64-bit-2025-06-07-12-37-18](https://github.com/user-attachments/assets/8fa5f3a8-2d64-493d-9be8-6ce06309a2a2)
### 10.Viewed compliance and MITRE ATT&CK mapping
![Ubuntu 64-bit-2025-06-07-12-38-54](https://github.com/user-attachments/assets/ee31fb80-072f-449b-90bd-615fffcbf539)
### 11.Verified PCI DSS rules and vulnerability detection
![Ubuntu 64-bit-2025-06-07-12-39-23](https://github.com/user-attachments/assets/da549567-7dcd-4fe1-92ec-5c32e6a61bdb)

## To start or stop all Wazuh services at once (Manager + Agent + Dashboard + Filebeat/Elasticsearch if installed)

###  ✅ Step 1: Create Script File
#### **```nano manage_wazuh.sh```**
###  ✅ Step 2: Paste the following content

bash
```Action: start or stop
ACTION=$1

if [[ "$ACTION" != "start" && "$ACTION" != "stop" && "$ACTION" != "restart" ]]; then
  echo "Usage: $0 {start|stop|restart}"
  exit 1
fi

echo "Performing '$ACTION' on all Wazuh services..."

Wazuh Manager

sudo systemctl $ACTION wazuh-manager

Wazuh Dashboard

sudo systemctl $ACTION wazuh-dashboard

Wazuh Agent (if running on same machine)

sudo systemctl $ACTION wazuh-agent

Filebeat (optional, if installed)

sudo systemctl $ACTION filebeat

Elasticsearch (optional)

sudo systemctl $ACTION elasticsearch

echo "All services have been $ACTIONed."```

### ✅ Step 3: Make it Executable
#### **```chmod +x manage_wazuh.sh```**

### ✅ Step 4: Run the Script
#### **```./manage_wazuh.sh start```**

#### **```./manage_wazuh.sh stop```**

#### **```./manage_wazuh.sh restart```**



