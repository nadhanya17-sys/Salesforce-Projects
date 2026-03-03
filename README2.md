# Wallet Management System – Salesforce App Builder Project

## Project Overview
Designed and implemented a Wallet Management module in Salesforce to manage users, their wallets, and associated bills.

This project demonstrates custom object creation, Lightning App configuration, and application-level customization.

##  Business Requirement
The company required a system to:
- Maintain digital wallets for users
- Track bills associated with each wallet
- Provide easy access through a dedicated Lightning App

##  Solution Implementation

###  Custom Objects Created

####  User (Custom Object)
- Fields:
  - User Name
  - Email
  - Phone Number
- Relationship:
  - One User → Many Wallets

####  Wallet (Custom Object)
- Fields:
  - Wallet Balance
  - Wallet ID
  - Status (Active/Inactive)
- Relationship:
  - One Wallet → Many Bills
  - Lookup to User

####  Bill (Custom Object)
- Fields:
  - Bill Amount
  - Bill Date
  - Payment Status
- Lookup to Wallet

###  Custom Tabs
Created custom tabs for:
- User
- Wallet
- Bill

Enabled visibility through profile settings.

###  Lightning App Creation
Created a custom Lightning App named:
"Wallet Management App"

Included:
- User
- Wallet
- Bill
- Reports

Configured navigation style and branding.

###  App Launcher Access
Assigned app visibility through profile.
Verified that users can access the Wallet Management App from App Launcher.

## Salesforce Features Used
- Custom Objects
- Lookup Relationships
- Lightning App Builder
- Custom Tabs
- Profiles
- App Launcher Configuration
  
## Screenshots
<img width="686" height="265" alt="image" src="https://github.com/user-attachments/assets/0175d686-da5e-41f7-a4d3-349ec51f328b" />
<img width="621" height="300" alt="image" src="https://github.com/user-attachments/assets/e4786e4d-91ca-4919-883d-70c81ee00d19" />
<img width="529" height="301" alt="image" src="https://github.com/user-attachments/assets/cf9f2442-b5db-4e3e-8d31-3b19552d694a" />


