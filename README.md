#  Secure Azure Web App + SQL Integration

This project demonstrates how to securely connect an **Azure Web App (.NET)** to an **Azure SQL Database** using **Private Endpoints**, **Virtual Networks (VNet)**, and **custom DNS**—eliminating all public exposure.

---

## 🧠 Overview

The solution follows best practices for secure network communication in Azure by:
- Hosting the Web App inside an **App Service Environment** connected to a **VNet**.
- Using **Private Link** to connect to the SQL Database without a public IP.
- Implementing **custom DNS resolution** to route traffic through private endpoints.
- Enforcing **Zero Trust** by denying public network access to Azure SQL.

---

## Diagram
<img width="951" height="546" alt="Screen Shot 2025-07-30 at 6 51 37 PM" src="https://github.com/user-attachments/assets/392bdeae-2f3e-43a8-9d6d-bee240028bcd" />


**Components:**
- **Azure App Service** – Hosts the web application (.NET).  
- **Azure SQL Database** – Backend data store, accessible only via Private Endpoint.  
- **Private Endpoint** – Provides secure, private connectivity between the app and database.  
- **Virtual Network (VNet)** – Isolates network traffic between resources.  
- **DNS Zone** – Ensures name resolution for the private endpoint.

---

## ⚙️ Deployment Steps

1. Create a resource group and VNet in Azure.  
2. Deploy Azure App Service and Azure SQL Database.  
3. Configure **Private Endpoint** for the SQL Database.  
4. Set up **Private DNS Zone** and link it to the VNet.  
5. Deploy **Bicep template** (optional) for automated IaC setup.  
6. Verify private connectivity via `nslookup` and Azure Portal diagnostics.

---

## 🧠 Skills Demonstrated
- Azure App Service Deployment  
- Azure SQL Private Link Configuration  
- Secure Networking (VNet + DNS + NSG)  
- Infrastructure as Code (Bicep)  
- Zero Trust Design  

---


