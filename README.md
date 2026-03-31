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

## Validation

This project was validated by confirming:
successful SSH access to the VM
Nginx was active and enabled
the custom HTML page loaded in a web browser
HTTP traffic was allowed
SSH access was restricted to a trusted IP

## Troubleshooting

## Issue: Could not reach the hosted page
Possible causes:
- HTTP was not allowed in the NSG
- Nginx was not running 
- the public IP address changed or was entered incorrectly

## Issue: SSH connection failed
Possible causes:
- wrong username
- incorrect SSH key path
- SSH source IP not allowed in the NSG
- VM not running

## What I Learned

- deploying and managing a Linux VM in Azure
- using SSH key authentication for secure remote access
- managing Linux services with systemctl
- understanding how Azure NSG rules affect connectivity and security
- hosting and updating a static webpage with Nginx


## About This Project

I built this project to strengthen my entry-level cloud and Linux administration skills through a practical hands-on lab. It reflects the kind of setup and troubleshooting tasks that appear in junior IT, support, and cloud-focused roles.

## License

This project was created for educational and portfolio purposes.
