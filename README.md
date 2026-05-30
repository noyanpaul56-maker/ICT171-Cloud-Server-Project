# ICT171 Cloud Server Project

## Student Information
Student Name: Noyon Chandra Paul
Student Number: 35916323

## Website Information
Domain Name: noyonchandrapaul.online
Public IP Address: 20.255.57.88

## Project Overview
This project demonstrates the deployment of a cloud-hosted website using Microsoft Azure Virtual Machines.

### Purpose
This script displays system information including hostname, date, memory usage and disk usage.


```bash
#!/bin/bash
hostname
date
df -h
free -h
## Azure Virtual Machine Setup
- Ubuntu Linux Virtual Machine
- Hosted on Microsoft Azure
- Public IP assigned

## DNS Configuration
- Domain purchased and configured
- DNS records pointed to Azure VM public IP

## Web Server
- Nginx installed and configured

## SSL/TLS Configuration
- Let's Encrypt SSL certificate installed using Certbot
- HTTPS enabled successfully

## Website URL
https://noyonchandrapaul.online
