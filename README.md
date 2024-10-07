# Ansible Automation for Infrastructure

This repository contains Ansible playbooks and roles used to automate personal infrastructure projects. It reflects my journey in learning and applying Infrastructure as Code (IaC), including setups for web servers, databases, and local development environments.

## Repository Overview

- **`ansible-roles/`**: Reusable roles (managed as a submodule) for common tasks like server provisioning and software installation.
  
- **`inventories/`**: Host and environment definitions:
  - **Production**: Inventory for live environments.
  - **Staging**: Pre-production environment for testing.
  - **Local**: Configurations for localhost or development VMs.

- **`playbooks/`**: Core infrastructure playbooks, designed to deploy and manage servers.
  
- **`ansible_quickstart/`**: Ignored experimental content from my Ansible learning process.

## How to Use

### Prerequisites

Ensure Ansible is installed:

```bash
sudo apt install ansible      # Ubuntu/Debian
brew install ansible          # macOS
```

### Running Playbooks
Specify inventory file and playbook:
```bash
ansible-playbook -i inventories/production playbooks/webserver_setup.yml
```

## Contributing
Open to contributions. Feel free to fork, submit issues, or create pull requests for improvements.

