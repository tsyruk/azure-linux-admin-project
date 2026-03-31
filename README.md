# Azure Linux Admin Project

Azure cloud administration project focused on deploying and securing an Ubuntu virtual machine with SSH, Network Security Group rules, Nginx, and static web hosting.

## Overview

This project demonstrates foundational cloud and Linux administration skills by deploying an Ubuntu virtual machine in Microsoft Azure, configuring secure remote access, installing and managing Nginx, and hosting a public-facing static webpage.

The goal was to build a small but realistic hands-on lab that shows basic server setup, connectivity, security, and web hosting.

## Skills Demonstrated

- Azure virtual machine deployment
- Linux server administration
- SSH remote access with key-based authentication
- Nginx installation and service management
- Azure Network Security Group configuration
- Static website hosting
- Basic troubleshooting and validation

## Environment

- Microsoft Azure
- Azure for Students
- Ubuntu 24.04 LTS
- Nginx
- PowerShell
- SSH

## Project Goals

- Deploy a Linux VM in Azure
- Connect securely using SSH keys
- Install and configure Nginx
- Host a custom HTML webpage
- Allow HTTP access while restricting SSH access
- Validate that the server is reachable and functioning correctly

## Project Steps

1. Created an Ubuntu Linux virtual machine in Azure
2. Configured SSH public key authentication
3. Connected to the server remotely with SSH
4. Updated the system packages
5. Installed Nginx
6. Verified the Nginx service was running and enabled
7. Replaced the default Nginx page with a custom HTML webpage
8. Configured NSG rules to allow HTTP traffic
9. Restricted SSH access to a trusted public IP
10. Verified the site was reachable through the VM’s public IP

## Security Decisions

- Used SSH key authentication instead of password-based login
- Limited inbound access through Azure NSG rules
- Allowed HTTP for public web access
- Restricted SSH to a trusted source IP to reduce exposure

## Commands Used

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install nginx -y
sudo systemctl status nginx
sudo systemctl enable nginx
sudo nano /var/www/html/index.html
