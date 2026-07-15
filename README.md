# 🌐 Hosting a Static Website on AWS EC2 with Amazon S3 Backup

## 📖 Project Overview

This project demonstrates how to deploy a static website on **Amazon Web Services (AWS)** using an **Amazon EC2** instance and **Apache HTTP Server**, while storing a backup of the website in **Amazon S3**.

The objective is to gain hands-on experience with cloud computing fundamentals, including virtual machines, web hosting, cloud storage, and basic network security.

---

## 🎯 Objectives

- Launch an Amazon EC2 instance.
- Install and configure Apache HTTP Server.
- Host a static HTML website.
- Configure Security Groups for secure access.
- Create an Amazon S3 bucket.
- Upload website backup files to S3.
- Understand the basics of AWS cloud services.

---

## ☁️ AWS Services Used

- **Amazon EC2** – Virtual server for hosting the website
- **Amazon S3** – Object storage for website backup
- **Security Groups** – Virtual firewall to manage inbound traffic
- **EC2 Instance Connect** – Browser-based SSH connection

---

## 🛠️ Technologies Used

- HTML5
- Apache HTTP Server (httpd)
- Amazon Linux 2023
- AWS EC2
- AWS S3

---

## 📂 Project Structure

```
AWS-Static-Website-Hosting/
│
├── index.html
├── README.md
├── screenshots/
│   ├── ec2-running.png
│   ├── apache-running.png
│   ├── website-output.png
│   ├── security-group.png
│   ├── s3-bucket.png
│   └── s3-upload.png
└── report/
    └── AWS_Mini_Project_Report.pdf
```

---

## 🚀 Project Workflow

1. Created an AWS account.
2. Launched an EC2 instance (Amazon Linux 2023).
3. Configured Security Group:
   - SSH (Port 22)
   - HTTP (Port 80)
4. Connected using EC2 Instance Connect.
5. Updated system packages.
6. Installed Apache HTTP Server.
7. Started and enabled Apache service.
8. Created a static `index.html` webpage.
9. Accessed the website using the EC2 Public IPv4 address.
10. Created an Amazon S3 bucket.
11. Uploaded the website backup (`index.html`) to S3.

---

## 💻 Commands Used

### Update the system

```bash
sudo dnf update -y
```

### Install Apache

```bash
sudo dnf install httpd -y
```

### Start Apache

```bash
sudo systemctl start httpd
```

### Enable Apache on boot

```bash
sudo systemctl enable httpd
```

### Check Apache status

```bash
sudo systemctl status httpd
```

### Navigate to web directory

```bash
cd /var/www/html
```

### Create website

```bash
sudo nano index.html
```

---

## 🌍 Website Access

The website is accessed through the **Public IPv4 Address** of the EC2 instance.

Example:

```
http://<Public-IP>
```

---

## 📸 Output

The project includes screenshots of:

- EC2 Instance (Running)
- Apache Server Status
- Website Output
- Security Group Configuration
- Amazon S3 Bucket
- Uploaded Website Backup

---

## 📈 Learning Outcomes

Through this project, I learned how to:

- Launch and manage EC2 instances.
- Install and configure Apache Web Server.
- Deploy a static website on AWS.
- Configure Security Groups.
- Store files using Amazon S3.
- Understand basic cloud infrastructure and networking.

---

## 🔒 Security Configuration

| Rule | Port | Source |
|------|------|--------|
| SSH | 22 | 0.0.0.0/0 |
| HTTP | 80 | 0.0.0.0/0 |

---

## 📌 Future Enhancements

- Deploy a dynamic website.
- Configure HTTPS using SSL/TLS.
- Register a custom domain with Amazon Route 53.
- Implement Auto Scaling.
- Use an Elastic Load Balancer (ELB).
- Automate deployments using CI/CD.

---

## 📚 References

- AWS Documentation: https://docs.aws.amazon.com/
- Amazon EC2 User Guide
- Amazon S3 User Guide
- Apache HTTP Server Documentation

---

## 👩‍💻 Author

**Radha**

B.Tech – Artificial Intelligence & Data Science

---

## ⭐ Acknowledgement

This project was completed as part of a Cloud Computing mini project to gain practical experience with Amazon Web Services (AWS), web hosting, and cloud storage.
