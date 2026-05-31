# Cloud Server Project Implementation

## Cloud Platform Selection

For this project, Microsoft Azure was selected as the cloud service provider. Azure was chosen because  students  credits through the Azure for Students program, allowing practical experience with Infrastructure as a Service (IaaS) technologies without additional hosting costs.

The project was implemented using Microsoft Azure Virtual Machines running Ubuntu Linux Server.

---

## Azure Account Setup

I registered for Microsoft Azure using my Murdoch University student account and activated the Azure for Students subscription.

Benefits included:

* Free Azure student credits
* Access to Virtual Machines
* Networking resources
* Public IP addresses
* Cloud storage and management tools

This subscription allowed me to deploy and manage a cloud server entirely through the Azure Portal.

---

## Virtual Machine Deployment

A new Ubuntu Linux Virtual Machine was created in Microsoft Azure.

### Configuration Details

| Setting           | Value                              |
| ----------------- | ---------------------------------- |
| Cloud Provider    | Microsoft Azure                    |
| Subscription Type | Azure for Students                 |
| Region            | East Asia                          |
| Operating System  | Ubuntu Server 24.04 LTS            |
| Deployment Model  | Infrastructure as a Service (IaaS) |
| Authentication    | SSH                                |
| Public IP         | 20.255.57.88                       |

The East Asia region was selected because it was available under my student subscription and provided sufficient resources for hosting the website.

After deployment, Azure automatically provisioned the virtual machine and assigned a public IP address, allowing remote administration through SSH.

---

## Server Access

The server was accessed remotely using Secure Shell (SSH).

Example connection:

```bash
az ssh vm --resource-group noyon_group_04171830 --vm-name noyon
```

SSH allowed secure command-line administration of the Linux server from any location.

---

## Domain Name Registration

To provide a professional online presence, a custom domain name was purchased.

### Domain Information

| Item                | Value                   |
| ------------------- | ----------------------- |
| Registrar           | Namecheap               |
| Domain              | noyonchandrapaul.online |
| Cost                | USD $1.65               |
| Registration Period | 1 Year                  |

The domain was purchased from Namecheap because of its low cost and simple DNS management interface.

---

## DNS Configuration

After purchasing the domain, DNS records were configured through the Namecheap DNS management console.

### DNS Record

| Record Type | Host | Value        |
| ----------- | ---- | ------------ |
| A Record    | @    | 20.255.57.88 |

The DNS A Record was configured to point the domain name to the Azure Virtual Machine's public IP address.

After DNS propagation, visitors could access the website using:

https://noyonchandrapaul.online

instead of using the server IP address directly.

---

## Web Server Installation

Nginx was installed as the web server software.

Commands used:

```bash
sudo apt update
sudo apt install nginx -y
```

Nginx was selected because it is lightweight, fast, secure and commonly used in modern cloud deployments.

---

## Website Deployment

The portfolio website files were uploaded to:

```bash
/var/www/html
```

The website was developed using:

* HTML5
* CSS3
* Responsive design principles

The website contains:

* Personal Profile
* Education Information
* Technical Skills
* Cloud Server Project Details
* Contact Information

---

## SSL/TLS Configuration

HTTPS was enabled to secure communication between visitors and the website.

SSL/TLS certificates were configured, allowing encrypted access to the site.

Secure website URL:

https://noyonchandrapaul.online

This protects user traffic and improves website trustworthiness.

---

## Skills Demonstrated

Through this project I gained practical experience in:

* Microsoft Azure Cloud Computing
* Linux Server Administration
* SSH Remote Management
* DNS Configuration
* Domain Management
* Nginx Web Server Administration
* SSL/TLS Security
* Website Hosting
* GitHub Documentation

This project demonstrates the deployment and management of a real-world cloud-hosted web server using Infrastructure as a Service technologies.

