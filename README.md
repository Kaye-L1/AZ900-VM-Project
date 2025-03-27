Azure Virtual Machine Deployment - AZ-900 Project

## Overview
This project demonstrates the process of deploying a **Virtual Machine (VM)** on Azure, connecting to it via **RDP (Remote Desktop Protocol)**, and then deleting it to prevent further charges. The project was completed as part of preparation for the **AZ-900: Microsoft Azure Fundamentals** certification.

## Steps
### 1. Create a Virtual Machine
- **Subscription:** Use your Azure subscription.
- **Resource Group:** Created a new resource group named `AZ900-VM-Project`.
- **VM Name:** `AZ900-VM-Demo`.
- **Region:** Choose a region close to your location for better latency.
- **Availability Options:** No infrastructure redundancy required.
- **Image:** Used **Windows Server 2022** for this deployment (or **Ubuntu** for Linux).
- **Size:** Selected the cheapest size: **B1s**.
- **Authentication Type:** Username and password authentication.
  - Username: `azureuser`
  - Password: A strong password.

### 2. Configure Networking
- **Virtual Network (VNet):** Let Azure create a default virtual network.
- **Subnet:** Kept the default subnet.
- **Public IP:** Allowed Azure to assign a public IP for remote connection.
- **Network Security Group (NSG):** Allowed inbound RDP (3389) for Windows, or SSH (22) for Linux.

### 3. Connect to the Virtual Machine
- **Windows VM:** 
  - Downloaded the RDP file from the Azure portal.
  - Used RDP to connect to the VM by providing the username and password.
- **Linux VM:** 
  - If using Linux, copy the SSH command from the Azure portal and connect via the terminal.

### 4. Deleting the Virtual Machine
- After testing the VM, I deleted the entire **Resource Group** (`AZ900-VM-Project`) to avoid unnecessary charges.
- This process also removes all associated resources (VM, networking, storage).

## Project Outcome
This project helped me practice the deployment, configuration, and deletion of an Azure Virtual Machine. I gained hands-on experience with Azure Compute, networking, and basic security configurations.

## Cost Control
- I selected the **B1s VM size** to minimize cost and deleted the VM immediately after the demonstration.
- The project was completed using a **pay-as-you-go** Azure plan, and no ongoing charges were incurred after VM deletion.

## Screenshots
- **Screenshot 1:** VM running on my local machine.

## Conclusion
This project provided foundational experience in Azure's compute and networking services. Understanding how to deploy and manage VMs will be useful for various Azure certifications and real-world IT roles.





___

Azure Storage Account - AZ-900 Project

## Overview
This project demonstrates the creation of an **Azure Storage Account** to understand cloud storage concepts.

## Steps
1. **Go to Azure Portal** and search for **Storage Accounts**.
2. Click **+ Create** to start the setup.
3. **Choose Subscription & Resource Group** (Create a new resource group if needed).
4. **Configure Storage Account:**
   - **Name:** az900storage-[your initials]
   - **Region:** (Choose the same as your previous resources)
   - **Performance:** Standard
   - **Redundancy:** Locally-redundant storage (LRS)
5. Click **Review + Create** and wait for the deployment to complete.
6. Once created, navigate to the **Storage Account Overview Page** to see your newly created resource.

## Screenshots:
- **Screenshot 1:** Created storage account.

## Key Learnings
- How to create and configure an Azure Storage Account.
- Understanding storage performance and redundancy options.
- Managing cloud storage resources in Azure.



