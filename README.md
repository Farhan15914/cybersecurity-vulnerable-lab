# Cybersecurity Vulnerable Lab

A deliberately vulnerable web application built for learning and demonstrating common web security vulnerabilities from the OWASP Top 10.

This project is designed for cybersecurity students and beginners to understand how vulnerabilities work and how attackers exploit them.

---

## Project Overview

This vulnerable lab contains intentionally insecure code to demonstrate real-world web security issues. It can be used for:

- Cybersecurity training
- Ethical hacking practice
- Security testing demonstrations
- Understanding OWASP Top 10 vulnerabilities

---

## Technologies Used

- PHP
- MySQL
- HTML
- CSS
- JavaScript
- Apache Server
- Ubuntu Linux

---

## Implemented Vulnerabilities

This lab currently contains the following vulnerabilities:

### 1. SQL Injection
Allows attackers to manipulate database queries through user input fields.

Example attack:' OR '1'='1' -- 

Impact:
- Unauthorized login
- Database data leakage

---

### 2. Cross-Site Scripting (XSS)

User input is not sanitized, allowing attackers to inject malicious JavaScript.

Example payload:
<script>alert('XSS')</script>

Impact:
- Session hijacking
- Cookie theft

---

### 3. Broken Authentication

Weak authentication mechanisms allow attackers to bypass login security.

Impact:
- Unauthorized account access
- Credential compromise

---

### 4. Cross-Site Request Forgery (CSRF)

The application does not validate request origins, allowing attackers to force users to perform unintended actions.

Impact:
- Unauthorized transactions
- Account manipulation

---

### 5. Server-Side Request Forgery (SSRF)

The server fetches URLs without proper validation, allowing attackers to access internal services.

Impact:
- Access internal systems
- Network reconnaissance

---

## Installation Guide

### Step 1
Install dependencies:
sudo apt update
sudo apt install apache2 mysql-server php php-mysql

### Step 2
Clone repository:
git clone https://github.com/Farhan15914/cybersecurity-vulnerable-lab.git

### Step 3
Move project to Apache directory:
sudo mv cybersecurity-vulnerable-lab /var/www/html/

### Step 4
Start Apache:
sudo systemctl start apache2

### Step 5
Access the website:
http://localhost/cybersecurity-vulnerable-lab

---

## Educational Purpose Only

This project was created strictly for **educational and cybersecurity training purposes**.

Do not deploy this application on a public server.

---

## Author

Farhan Bahadure  
Cybersecurity Student

GitHub:
https://github.com/Farhan15914

---

## Future Improvements

- Add more OWASP vulnerabilities
- Add penetration testing walkthrough
- Add security fixes demonstration
- Integrate logging and monitoring
