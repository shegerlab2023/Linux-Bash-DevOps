# Linux-Bash-DevOps

# Nginx Installation and Configuration Guide

Nginx is a popular web server known for its lightweight nature and versatility. This guide will walk you through the installation and basic configuration of Nginx on an Ubuntu 20.04 server.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Step 1: Installing Nginx](#step-1-installing-nginx)
- [Step 2: Adjusting the Firewall](#step-2-adjusting-the-firewall)
- [Step 3: Checking your Web Server](#step-3-checking-your-web-server)

## Prerequisites

Before you begin, ensure you have:

- An Ubuntu 20.04 server
- A regular user with sudo privileges
- Optional: A registered domain name for advanced configurations

## Step 1: Installing Nginx

Update your package repositories and install Nginx:

```bash
sudo apt update
sudo apt install nginx
```

## Step 2: Adjusting the Firewall

Allow HTTP traffic to access Nginx:

```bash
sudo ufw allow 'Nginx HTTP'
```

Verify the change:

```bash
sudo ufw enable
sudo ufw status
```

## Step 3: Checking your Web Server

Check if Nginx is running:

```bash
systemctl status nginx
```

Access the default Nginx landing page by entering your server's IP address in your browser:

```plaintext
http://your_server_ip or http://localhost:80
```

## Conclusion

You've successfully installed and configured Nginx on your Ubuntu 20.04 server. For advanced configurations and hosting multiple domains, refer to the official Nginx documentation.

Happy web serving!
```

