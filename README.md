# AWS EC2 Hello World Web Server

This project demonstrates deploying a simple web server on AWS EC2 using Ubuntu and Nginx.

## Services Used

* AWS EC2
* Ubuntu Server
* Nginx

## Steps Performed

1. Created EC2 instance
2. Selected Ubuntu AMI
3. Configured security groups
4. Allowed HTTP and SSH traffic
5. Used User Data script for automation
6. Installed and started Nginx
7. Hosted a Hello World webpage

## User Data Script

```bash
#!/bin/bash
apt update -y
apt install nginx -y
systemctl start nginx
systemctl enable nginx
echo "Hello World" > /var/www/html/index.html
```

## Output

Successfully deployed a web server on AWS EC2 and accessed it using the public IPv4 address.

## Screenshots

* EC2 instance running
* Browser output showing Hello World
