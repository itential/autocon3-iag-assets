# Playbook Requirements

This directory contains specific requirements files for each Ansible playbook.

## Installing Requirements

To install the requirements for a specific playbook, use:

```bash
pip install -r requirements/playbook-name.txt
```

## Collection Installation

After installing Python dependencies, you'll need to install the required Ansible collections:

```bash
ansible-galaxy collection install -r requirements/playbook-name.txt
```

## Available Requirements Files

- `ios-interface-description.txt`: Requirements for configuring Cisco IOS interface descriptions
- `cisco-nxos-vlan-config.txt`: Requirements for configuring VLANs on Cisco NX-OS switches

## General Notes

- Each requirements file includes both Python package dependencies and required Ansible collections
- The base Ansible requirements are included in each file for standalone installation
- Collection dependencies are listed as comments and should be installed with ansible-galaxy