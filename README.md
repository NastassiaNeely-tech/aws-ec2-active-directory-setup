# AWS Lab: Configuring Active Directory on EC2 (Domain Controller Setup)

## 📌 Overview
This lab demonstrates how to configure Active Directory Domain Services (AD DS) on a Windows EC2 instance. The server will be promoted to a domain controller and configured with a new forest.

---

## 🎯 Objective
- Install Active Directory Domain Services (AD DS)
- Promote a Windows Server to a Domain Controller
- Create a new Active Directory forest and domain

---

## 🎥 Video Walkthrough
[Click here to watch the Loom walkthrough] https://www.loom.com/share/111184ade5174c188b9e56278eb37eb6

---

## 🛠️ Technologies Used
- AWS EC2 (Windows Server)
- Active Directory Domain Services (AD DS)
- Windows Server Manager

---

## 🧠 Key Skills Demonstrated
- Windows Server administration
- Active Directory installation and configuration
- Domain controller promotion
- Forest and domain creation
- Identity and access management fundamentals

---

## 📸 Key Visual Highlights

### 1. Server Manager Dashboard
<img width="1908" height="962" alt="Server-manager" src="https://github.com/user-attachments/assets/9f1da938-4d8d-4a72-bd2a-721582a93786" />

### 2. Add Roles and Features Wizard
<img width="1883" height="965" alt="Roles-and-features" src="https://github.com/user-attachments/assets/2ab795bb-951a-4950-95ac-867aadcaac78" />

### 3. Selecting Active Directory Domain Services
<img width="1892" height="984" alt="ADDS-selection" src="https://github.com/user-attachments/assets/a2b4a771-56fd-4b55-8c89-890671fd4882" />

### 4. Promote Server to Domain Controller
<img width="1902" height="986" alt="Promote-server" src="https://github.com/user-attachments/assets/681d9810-10d2-43dc-9dca-9f7ac520a18c" />

### 5. Domain Configuration (adlab.local)
<img width="1909" height="974" alt="Domain-config" src="https://github.com/user-attachments/assets/ffea2f77-0cc3-4df2-8e14-d96571390f9a" />

### 6. Prerequisites Check Passed
<img width="1905" height="962" alt="Prereq-passed" src="https://github.com/user-attachments/assets/f0c997de-fc16-4002-b35b-a3c7c3a4ed17" />

---

## 🔄 Full Step-by-Step Process

### 1. Open Start Menu
- Click the **Windows icon** at the bottom of the screen

### 2. Open Server Manager
- Click **Server Manager**

### 3. Add Roles and Features
- Click **Add Roles and Features**
- Leave all settings as default until reaching **Server Roles**

### 4. Select Active Directory Domain Services
- Check **Active Directory Domain Services**
- Click **Next** through all default settings
- Click **Install**

### 5. Complete Installation
- Wait approximately **10 minutes**
- Once complete, click **Close**

### 6. Promote to Domain Controller
- Click the **flag icon** at the top
- Select **Promote this server to a domain controller**

### 7. Create New Forest
- Select **Add a new forest**
- Enter root domain name: **adlab.local**
- Click **Next**

### 8. Set DSRM Password
- Create a **Directory Services Restore Mode (DSRM)** password
- Ensure both entries match
- Click **Next**

### 9. Leave Defaults
- Continue clicking **Next** while leaving all settings as default

### 10. Verify Domain Name
- Confirm NetBIOS domain name (**ADLAB**) auto-populates
- Click **Next**

### 11. Prerequisites Check & Install
- Leave all settings default
- Wait for **Prerequisites Check**
- Once it shows **passed successfully**, click **Install**
- The system will prompt a **restart**

### 12. Reboot & Completion
- After reboot, Active Directory is fully configured
- The server is now a **Domain Controller**

---

## 🔐 Security Considerations
- Use a strong DSRM password and store it securely  
- Limit administrative access to the domain controller  
- Regularly update and patch the server  
- Follow least privilege principles for domain accounts  

---

## 🚀 Outcome
Successfully installed Active Directory Domain Services and promoted a Windows EC2 instance to a Domain Controller with a new forest (**adlab.local**).
