# Active Directory Home Lab
Windows Server Active Directory home lab demonstrating domain services, DHCP, user management, domain joining, and administrative troubleshooting 
## Overview

This project demonstrates the deployment and configuration of
Microsoft Active Directory Domain Services in a virtualized lab
environment.

The lab was designed to develop hands-on experience with Windows
Server administration, identity management, networking, and
enterprise IT support.

## Technologies Used

- Windows Server 2019
- Windows 10
- Windows 11
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- VirtualBox
- PowerShell
- TCP/IP networking

## Lab Architecture
The lab was built in Oracle VirtualBox and consists of Windows Server domain controller and Windows client machines.
### Domain Controller
- Windows Server 2019
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Domain: mydomain.com
### Client Machines
**CLIENT1**
- Windows 10  x64
- Connected to the internal virtual network
- Joined to the Active Directory domain
  
**CLIENT2**
- Windows 11 x64
- Used as an additional Windows client for testing and administration
## Network Architecture
The Domain Controller provides Active Directory, DNS, and DHCP services to the Windows client machines on the internal virtual network.
Domain controller > Internal Network > CLIENT1 / CLIENT2
    
## Lab Implementation

### 1. Windows Server Deployment

Installed Windows Server 2019 in VirtualBox and configured the
server's network interfaces.

[Screenshot]

### 2. Active Directory Installation

Installed Active Directory Domain Services and promoted the server
to a domain controller.

Domain created:

mydomain.com

[Screenshot]

### 3. DHCP Configuration

Configured DHCP to automatically provide network configuration to
client machines.

[Screenshot]

### 4. User Management

Created Active Directory user accounts and tested authentication
using domain credentials.

[Screenshot]

### 5. Domain Join

Connected Client1 to the internal network and successfully joined
the workstation to mydomain.com.

[Screenshot]

### 6. Domain Authentication

Verified that a domain user could authenticate to Client1 using
Active Directory credentials.

[Screenshot]

## Troubleshooting

During the lab, I encountered issues with domain authentication and
client connectivity.

I used tools such as:

- ipconfig
- ping
- nslookup
- Active Directory Users and Computers
- Windows network settings

to verify network connectivity, DNS configuration, and domain
membership.

## Skills Demonstrated

- Active Directory administration
- Windows Server administration
- User and computer management
- Domain authentication
- DHCP configuration
- DNS troubleshooting
- TCP/IP networking
- Virtual machine administration
- Help desk troubleshooting

## Future Improvements

- Implement Group Policy Objects (GPOs)
- Automate user creation with PowerShell
- Configure account lockout and password policies
- Create security groups and organizational units
- Implement role-based access control
- Connect Active Directory to Microsoft Entra ID
