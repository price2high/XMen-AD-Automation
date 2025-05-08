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

- xmen_users.csv # Contains user info (FirstName, LastName, Username)
- create_xmen_users.ps1 # Script to create AD users
- dd_users_to_group.ps1 # Script to add users to a group
- README.md # Project documentation

---
## 📈 Outcome

- ✅ Successfully created 70 Active Directory users using X-Men character data.
- ✅ Each user was assigned a real first and last name, with their X-Men code name used as the username.
- ✅ All users were added to a centralized AD group (`XMenTeam`) for easier management.
- ✅ Demonstrated the use of PowerShell for real-world IT automation tasks including:
  - CSV-based user provisioning
  - Secure password setting
  - Organizational Unit placement
  - Group membership assignment

---

## 🚀 Future Enhancements

- 🔐 Add error handling and logging to track account creation issues.
- 🔑 Generate and export randomized passwords securely to an encrypted admin file.
- 🗂️ Expand user attributes such as department, job title, and email.
- ☁️ Integrate with Azure Active Directory for hybrid or cloud environments.
- 📋 Build a GUI front-end for non-technical admins to trigger the script with a file upload.
- 🧪 Add unit tests or script validation before execution to catch errors early.

