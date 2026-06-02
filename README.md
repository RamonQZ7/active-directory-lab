# Active Directory Home Lab

## Overview
This project documents an Active Directory home lab built with Oracle VirtualBox, Windows Server, and a Windows 11 client virtual machine. The goal was to practice domain setup, user and group management, DNS configuration, domain joining, and basic troubleshooting.

## Lab Environment

| Component | Purpose |
|---|---|
| Oracle VirtualBox | Virtualization platform |
| Windows Server 2022 | Domain Controller, DNS, Active Directory Domain Services |
| Windows 11 Pro N | Domain-joined client workstation |
| Internal Network | Private lab network between server and client |

## Network Configuration

| Device | IP Address | Role |
|---|---|---|
| Windows Server | 192.168.10.10 | Domain Controller / DNS |
| Windows 11 Client | 192.168.10.20 | Domain-joined workstation |

Domain name: `lab1.local`

## What I Configured

- Installed Windows Server 2022 in VirtualBox
- Configured a static IP address on the server
- Installed Active Directory Domain Services
- Promoted the server to a domain controller
- Created the `lab1.local` domain
- Created OUs for IT, HR, and Sales
- Created domain users and security groups
- Added users to their correct groups
- Installed a Windows 11 client VM
- Configured client IP and DNS settings
- Joined the Windows 11 client to the domain
- Logged into the Windows 11 client using a domain user account
- Verified the lab using `ping`, `nslookup`, `net user`, `net group`, and `whoami`

## Skills Practiced

- Active Directory Domain Services
- Domain Controller setup
- DNS configuration
- Static IP addressing
- Windows Server administration
- Windows client domain join
- Organizational Units
- User and group management
- Command-line verification and troubleshooting

## Screenshots

Screenshots are located in the `/screenshots` folder.

## Future Improvements

- Configure shared folder permissions by department
- Create Group Policy Objects
- Map network drives for domain users
- Add password policy and account lockout policy
