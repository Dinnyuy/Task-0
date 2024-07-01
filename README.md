# Stage-0
---

# Static Website Deployment on AWS EC2

This repository contains files and instructions for deploying a static website on AWS EC2 using NGINX as the web server.

## Website Details

- **Name:** Dinnyuy Lemnyuy Fru Angu
- **Username:** Dinnyuy L Fru Angu
- **Email:** dinnyuylemnyuy@gmail.com

## Project Files

- `index.html`: Main HTML file containing the structure and content of the static website.
- `styles.css`: CSS file for styling the website.
- `scripts.js`: JavaScript file for adding interactive elements to the website.

## Deployment Instructions

1. **Set Up AWS EC2 Instance**
   - Launch an EC2 instance with Ubuntu Server.
   - Configure security groups to allow HTTP (port 80) and SSH (port 22) access.

2. **Clone Repository and Install NGINX**
   - Clone this repository to your EC2 instance:
     ```bash
     git clone -b master https://github.com/Dinnyuy/Task-0.git
     ```
   - Install NGINX:
     ```bash
     sudo apt update
     sudo apt install nginx -y
     ```

3. **Configure NGINX**
   - Move website files to NGINX web server directory:
     ```bash
     sudo mv * /var/www/html/
     ```
   - Start and enable NGINX service:
     ```bash
     sudo systemctl start nginx
     sudo systemctl enable nginx
     ```

4. **Access Your Website**
   - Open your web browser and navigate to your EC2 instance's public IP address.



