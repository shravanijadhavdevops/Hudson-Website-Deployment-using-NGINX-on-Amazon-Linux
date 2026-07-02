# Hudson Website Deployment using NGINX on Amazon Linux
## Introduction
This is my first mini project where I deployed my website “Hudson” on an Amazon Linux server using NGINX.
The main goal of this project is to understand how website deployment works in a real environment. It includes setting up a server, installing NGINX, and hosting a static website so it can be accessed through an IP address.

## Technologies Used
* Amazon Linux (EC2)<br>
* NGINX Web Server<br>
* HTML, CSS<br>
* Linux Commands<br>

## Features
* Simple static website deployment<br>
* NGINX server configuration<br>
* Accessible through public/private IP<br>
* Beginner-friendly DevOps project<br>

## Architect Diagram
![alt text](image.png)


## Steps I Followed
### 1. Launch Amazon Linux Instance
* Created an EC2 instance<br>
![alt text](<imgs/create a instance.png>)  
* Connected using SSH
![alt text](<imgs/connect instance use ssh.png>)
### 2.Install NGINX
sudo yum update -y<br>
sudo yum install nginx -y
![alt text](<imgs/install nginx.png>)
### 3.Start NGINX Server
sudo systemctl start nginx<br>
sudo systemctl enable nginx
![alt text](<imgs/start nginx server.png>)
### 4.Deploy Website Files
* copied project files
![alt text](<imgs/copied project files.png>)
cd /usr/share/nginx/html

* Moved my website files to nginx directory.
![alt text](<imgs/moved website in nginx.png>)
### 5.Restart Server
sudo systemctl restart nginx
![alt text](<imgs/restart nginx.png>)
### 6. Access Website

* Open browser
* Enter Public IP of instance
* Website "Hudson" is live 🎉
![alt text](<imgs/acess website2.png>)

## What i Learned
* Basics of cloud computing
* How to configure NGINX
* How to deploy a website on server
* Linux command usage

## Project Summary
This project helped me gain practical knowledge of website deployment and gave me confidence to explore more in DevOps and Cloud Computing.