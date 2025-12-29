# SQL Injection Detection and Prevention Experiment using DVWA

## Overview
This repository contains the experimental materials used in the study titled:
**“Analysis of SQL Injection Attacks and Prevention Mechanisms using DVWA”**.

The experiments were conducted in a controlled local environment to evaluate:
- Manual SQL injection attacks
- Automated SQL injection exploitation using SQLMap
- The effectiveness of security configurations in preventing SQL injection

## Experimental Environment
- Operating System: Windows 10
- Web Server Stack: XAMPP (Apache, MySQL, PHP)
- Vulnerable Application: Damn Vulnerable Web Application (DVWA)
- Database: MySQL (MariaDB)
- Automation Tool: SQLMap

## Experiment Scope
The experiments compare SQL injection behavior under:
- **Low security configuration**
- **High security configuration**

Metrics observed include:
- SQL injection success/failure
- Data exposure
- Data integrity
- Access control effectiveness

## Reproducibility Steps
1. Install XAMPP and start Apache & MySQL
2. Deploy DVWA in the `htdocs` directory
3. Configure DVWA database
4. Set DVWA security level to **Low**
5. Perform manual SQL injection tests
6. Execute SQLMap commands listed in `sqlmap_commands.txt`
7. Set DVWA security level to **High**
8. Re-run SQLMap with flushed session data

## Repository Contents
- `sqlmap_commands.txt`: SQLMap commands used during the experiment
- `dvwa_setup.md`: DVWA installation and configuration steps
- `screenshots/`: Evidence screenshots corresponding to figures used in the report

## Disclaimer
This repository is intended **strictly for academic and educational purposes**.
All experiments were conducted in a local test environment.
