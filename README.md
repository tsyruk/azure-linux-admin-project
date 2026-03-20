# Azure Linux Admin Project

## Overview
This project demonstrates basic cloud and Linux administration skills by deploying an Ubuntu virtual machine in Microsoft Azure, configuring secure SSH access, installing Nginx, and hosting a public-facing static webpage.

## Skills Demonstrated
- Azure virtual machine deployment
- Linux server administration
- SSH remote access
- Nginx installation and service management
- Azure NSG configuration
- Basic web hosting

## Environment
- Microsoft Azure
- Azure for Students
- Ubuntu 24.04 LTS
- Nginx
- PowerShell / SSH

## Project Steps
1. Created an Ubuntu Linux virtual machine in Azure
2. Configured SSH public key authentication
3. Connected to the server remotely with SSH
4. Updated the system and installed Nginx
5. Verified the Nginx service was running and enabled
6. Replaced the default Nginx page with a custom HTML webpage
7. Configured NSG rules to allow HTTP and restrict SSH access
8. Verified the site was accessible through the VM’s public IP

## Validation
- Confirmed successful SSH access to the VM
- Confirmed Nginx service was active and enabled
- Confirmed the custom webpage loaded in a browser
- Confirmed SSH access was restricted to a trusted public IP

## Screenshots
Azure VM Overview
- <img width="1709" height="848" alt="image" src="https://github.com/user-attachments/assets/d95fca13-d0b0-4dfb-bc23-f8a2cb211a68" />
Network Security Group rules
- <img width="1374" height="669" alt="image" src="https://github.com/user-attachments/assets/a6611ebf-9598-4389-8d63-4be37a48204c" />
SSH session + Nginx service status
- <img width="1571" height="375" alt="image" src="https://github.com/user-attachments/assets/67ecb4be-54fb-4838-951f-ba64b7cfb61e" />
Live hosted webpage
- <img width="1379" height="901" alt="image" src="https://github.com/user-attachments/assets/3c2112dd-3038-4ed2-89b4-8ad482a971bc" />


## Learned
- How to deploy and manage a Linux VM in Azure
- How SSH key authentication works
- How to manage Linux services with `systemctl`
- How Azure NSG rules affect connectivity and security
- How to host and update a static webpage with Nginx

## Working On
- Add HTTPS with Let's Encrypt
- Use a custom domain
- Automate deployment updates
- Expand the webpage into a fuller portfolio site
