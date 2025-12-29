# DVWA Setup and Configuration Guide

## Installation
1. Install XAMPP
2. Extract DVWA into `C:\xampp\htdocs\DVWA`
3. Start Apache and MySQL via XAMPP Control Panel

## Database Configuration
1. Navigate to `http://localhost/DVWA/setup.php`
2. Click "Create / Reset Database"
3. Confirm database creation success

## Database Privileges Configuration (phpMyAdmin)
To ensure proper database access for DVWA, database user privileges were configured using phpMyAdmin.

1. Access phpMyAdmin via `http://localhost/phpmyadmin`
2. Navigate to the **User accounts** tab
3. Select the database user configured for DVWA
4. Assign full privileges to the `dvwa` database, including:
   - SELECT
   - INSERT
   - UPDATE
   - DELETE
   - CREATE
   - DROP
   - ALTER

These privileges ensure DVWA functions correctly and that vulnerabilities observed during testing are due to insecure query handling rather than permission restrictions.

## Security Level Configuration
- Login to DVWA as `admin`
- Navigate to DVWA Security
- Set security level to:
  - Low for baseline testing
  - High for prevention evaluation

## SQL Injection Module
- Module path:
  `http://localhost/DVWA/vulnerabilities/sqli/`
- Tested parameter: `id`
