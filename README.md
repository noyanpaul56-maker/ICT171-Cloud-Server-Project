# Cloud Server Project Implementation

## Public Server Information

### Live Website

🌐 Website: https://noyonchandrapaul.online

### GitHub Repository

📂 Repository: https://github.com/noyanpaul56-maker/ICT171-Cloud-Server-Project

### Server Information

| Item              | Value                   |
| ----------------- | ----------------------- |
| Cloud Provider    | Microsoft Azure         |
| Operating System  | Ubuntu Server 24.04 LTS |
| Web Server        | Nginx                   |
| Domain Name       | noyonchandrapaul.online |
| Public IP Address | 20.255.57.88            |
| Security          | SSL/TLS (Let's Encrypt) |

---

## Cloud Platform Selection

For this project, Microsoft Azure was selected as the cloud service provider. Azure was chosen because students receive credits through the Azure for Students program, allowing practical experience with Infrastructure as a Service (IaaS) technologies without additional hosting costs.

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

### Azure Virtual Machine

![Azure VM](screenshots/01-azure-vm.png)

**Figure 1:** Azure Virtual Machine running in Microsoft Azure.

---

## Server Access

The server was accessed remotely using Secure Shell (SSH).

Example connection:

```bash
az ssh vm --resource-group noyon_group_04171830 --vm-name noyon
```

### SSH Access

![SSH Connection](screenshots/02-ssh-connection.png)

**Figure 2:** Successful SSH connection to the Ubuntu Linux server.

---

## Domain Name Registration

To provide a professional online presence, a custom domain name was purchased.

### Domain Information

| Item                | Value                   |
| ------------------- | ----------------------- |
| Registrar           | Namecheap               |
| Domain              | noyonchandrapaul.online |
| Cost                | AUD $1.65               |
| Registration Period | 1 Year                  |

The domain was purchased from Namecheap because of its low cost and simple DNS management interface.

---

## DNS Configuration

After purchasing the domain, DNS records were configured through the Namecheap DNS management console.

### DNS Record

| Record Type | Host | Value        |
| ----------- | ---- | ------------ |
| A Record    | @    | 20.255.57.88 |

### DNS Propagation Verification

![DNS Propagation](screenshots/05-dns-propagation.png)

**Figure 3:** DNS Checker confirms that the domain correctly resolves to the Azure VM public IP address.

---

## Web Server Installation

Nginx was installed as the web server software.

```bash
sudo apt update
sudo apt install nginx -y
```

### Nginx Service Status

![Nginx Status](screenshots/03-nginx-status.png)

**Figure 4:** Nginx service running successfully.

### Nginx Installation Verification

![Nginx Installation](screenshots/04-nginx-installation.png)

**Figure 5:** Package installation history confirming successful Nginx installation.

---

## Website Deployment

The portfolio website files were uploaded to:

```bash
/var/www/html
```

The website was developed using:

* HTML5
* CSS3
* Responsive Design

The website contains:

* Personal Profile
* Education Information
* Technical Skills
* Cloud Server Project Details
* Contact Information

---

## SSL/TLS Configuration

HTTPS was enabled to secure communication between visitors and the website.

### SSL Certificate Verification

![SSL Certificate](screenshots/06-ssl-certificate.png)

**Figure 6:** Let's Encrypt SSL certificate successfully installed and active.

Secure website URL:

https://noyonchandrapaul.online

---

## Final Website

![Portfolio Website](screenshots/07-final-website.png)

**Figure 7:** Final deployed cybersecurity portfolio website accessible through the custom domain.

---

## GitHub Repository

GitHub was used to store source code, screenshots and project documentation.

![GitHub Repository](screenshots/08-github-repository.png)

**Figure 8:** GitHub repository containing project files and documentation.

Repository:

https://github.com/noyanpaul56-maker/ICT171-Cloud-Server-Project

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

---

## Final Architecture Diagram

```text
User Browser
      ↓
Domain (Namecheap)
      ↓
DNS
      ↓
Azure VM (Ubuntu)
      ↓
Nginx Web Server
      ↓
Portfolio Website
      ↓
SSL (Let's Encrypt)
```

---

## Conclusion

This project demonstrates the deployment and management of a real-world cloud-hosted web server using Infrastructure as a Service technologies.
