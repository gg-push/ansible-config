# Secure Linux Server Ansible Playbook

## Overview
Configures a Linux server (Debian/Ubuntu or RedHat/CentOS) with cybersecurity best practices. It updates the system, creates a secure admin user, hardens SSH, sets up a firewall (UFW or firewalld), enables Fail2Ban, activates auditd, and disables insecure services.

## Features
- System updates and essential package installation
- Secure admin user with SSH key authentication
- SSH hardening (custom port, no root login, no password auth)
- Firewall configuration (UFW for Debian, firewalld for RedHat)
- Fail2Ban for brute-force protection
- Auditd for system auditing
- Disables telnet and FTP services

## Usage
1. Update `inventory.yml` with your server's IP or hostname.
2. Apply the playbook 

```bash
    ansible-playbook -i inventory.yml site.yml
```
