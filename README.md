# 🧬 X-Men Active Directory Automation with PowerShell

This project automates the creation of 70 Active Directory (AD) users using X-Men characters. It demonstrates how PowerShell can be used for real-world user provisioning and group membership automation using a CSV data source.

---

## 📄 Overview

**Features:**
- Creates Active Directory users from a CSV file
- Assigns realistic first and last names
- Uses X-Men code names as usernames
- Sets a default secure password
- Places users in a specific Organizational Unit (OU)
- Adds all users to a security group (`XMenTeam`)

---

## 🛠️ Technologies Used

- PowerShell
- Active Directory Module for Windows PowerShell
- CSV for data input
- Windows Server with AD DS

---

## 📁 Project Structure
XMen-AD-Automation/
├── xmen_users.csv # Contains user info (FirstName, LastName, Username)
├── create_xmen_users.ps1 # Script to create AD users
├── add_users_to_group.ps1 # Script to add users to a group
└── README.md # Project documentation

