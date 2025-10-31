#  Secure Azure Web App + SQL Integration

## 🧠 Overview

The solution follows best practices for secure network communication in Azure by:
- Hosting the Web App inside an App Service Environment connected to a VNet.
- Using Private Link to connect to the SQL Database without a public IP.
- Implementing custom DNS resolution to route traffic through private endpoints.
- Enforcing Zero Trust by denying public network access to Azure SQL.

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


## 🧠 Skills Demonstrated
- Azure App Service Deployment  
- Azure SQL Private Link Configuration  
- Secure Networking (VNet + DNS + NSG)  
- Infrastructure as Code (Bicep)  
- Zero Trust Design  

---


