# Changelog

All notable changes to this project will be documented in this file.

The project follows an incremental learning approach, with each sprint introducing new DevOps concepts and automation practices.

---

## Sprint 1 – Ansible Project Foundation (Completed)

### Added

- Created project directory structure.
- Initialized Git repository.
- Connected project to GitHub.
- Configured Ansible using `ansible.cfg`.
- Created static inventory with host groups:
  - webservers
  - dbservers
- Added project `.gitignore`.
- Established repository structure for:
  - roles
  - playbooks
  - templates
  - variables
  - inventories
  - files
  - documentation

### Skills Practiced

- Git
- GitHub
- WSL Linux environment
- Ansible installation
- YAML configuration
- Inventory management
- Ansible configuration
- Project organization

---

## Sprint 2 – AWS Infrastructure Automation (Completed)

### Added

- Created `feature/aws-provisioning` development branch.
- Verified AWS CLI authentication using IAM credentials.
- Verified AWS identity using AWS STS.
- Installed and verified the `amazon.aws` Ansible collection.
- Installed and verified Python `boto3` SDK.
- Configured AWS region:
  - `eu-central-1` (Frankfurt)

### AWS Key Pair Automation

- Created Ansible playbook to provision AWS EC2 Key Pair.
- Automated private key generation.
- Saved generated private key locally.
- Secured private key permissions using `0600`.
- Updated `.gitignore` to prevent committing sensitive files:
  - `.pem`
  - secrets
  - credentials

### AWS Security Group Automation

- Created reusable AWS variable file:

```text
group_vars/aws.yml


## Sprint 3 – Linux Baseline Automation

### Added

- Implemented Linux server baseline configuration using Ansible roles.
- Automated system package updates.
- Installed and configured Chrony time synchronization.
- Created DevOps administration user with sudo privileges.
- Implemented SSH hardening using Ansible lineinfile module.
- Added SSH handler to restart services only when configuration changes occur.
- Recovered from SSH configuration failure by improving automation approach.

### Skills Practiced

- Ansible roles
- Linux administration
- User management
- SSH security hardening
- Templates vs lineinfile
- Handlers
- Idempotent automation
- Troubleshooting failed deployments
- Infrastructure recovery
