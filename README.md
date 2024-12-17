# Ansible Projects for Windows and Ubuntu

This repository contains two Ansible projects:

## Windows Ansible Project
Located in `windows_ansible/` directory:
- Installs Google Chrome on Windows servers
- Uses WinRM for connection
- Requires proper Windows credentials and WinRM setup

### Usage:
```bash
ansible-playbook -i windows_ansible/inventory.ini windows_ansible/install_chrome.yml
```

## Ubuntu Ansible Project
Located in `ubuntu_ansible/` directory:
- Updates package cache
- Performs system update using apt
- Uses SSH for connection
- Requires SSH key authentication

### Usage:
```bash
ansible-playbook -i ubuntu_ansible/inventory.ini ubuntu_ansible/update_packages.yml
```

## Setup Instructions:
1. Update the inventory files with your server IP addresses
2. Configure proper credentials in inventory files
3. Ensure WinRM is set up on Windows servers
4. Ensure SSH access is configured for Ubuntu servers