# Ansible Playbook for Apache Server Setup

This repository contains an Ansible playbook designed to install and configure the Apache web server on a target host. The playbook ensures that the latest version of Apache and firewalld are installed, configures firewalld to allow HTTP traffic, and starts the Apache service.

## Table of Contents
- [Requirements](#requirements)
- [Usage](#usage)
- [Playbook Details](#playbook-details)
- [License](#license)

## Requirements

- Ansible installed on the control node.
- Target host(s) should be accessible via SSH and configured in the Ansible inventory.
- Target host(s) should be running a Linux distribution that supports the `yum` package manager (e.g., CentOS, RHEL).

## Usage

Update the inventory file: Ensure that your target hosts are listed in the inventory file under the [web] group.

Run the playbook: Execute the playbook using the following command:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/ansible-apache-setup.git
   cd ansible-apache-setup
ansible-playbook -i inventory apache_setup.yml


