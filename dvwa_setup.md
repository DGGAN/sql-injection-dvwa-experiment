# DVWA Setup and Configuration Guide

## Installation
1. Install XAMPP
2. Extract DVWA into `C:\xampp\htdocs\DVWA`
3. Start Apache and MySQL via XAMPP Control Panel

## Database Configuration
1. Navigate to `http://localhost/DVWA/setup.php`
2. Click "Create / Reset Database"
3. Confirm database creation success

## Security Level Configuration
- Login to DVWA as `admin`
- Navigate to DVWA Security
- Set security level to:
  - **Low** for baseline testing
  - **High** for prevention evaluation

## SQL Injection Module
- Access path:
  `http://localhost/DVWA/vulnerabilities/sqli/`
- Parameter tested: `id`
