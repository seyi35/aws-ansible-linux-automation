# Changelog

All notable changes to this project will be documented in this file.

The project follows an incremental learning approach, with each sprint introducing new DevOps concepts and automation practices.

---

## Sprint 2 – AWS Infrastructure Automation (In Progress)

### Added

* Created `feature/aws-provisioning` development branch.
* Verified AWS CLI authentication using IAM credentials.
* Installed and verified the `amazon.aws` Ansible collection.
* Installed and verified the Python `boto3` SDK.
* Configured AWS default region to `eu-central-1` (Frankfurt).
* Created an Ansible playbook to provision an AWS EC2 Key Pair.
* Stored the generated private key securely with restricted file permissions (`0600`).
* Updated `.gitignore` to prevent accidental commits of sensitive files such as SSH private keys.

### Skills Practiced

* AWS authentication
* Infrastructure as Code (IaC)
* Ansible AWS collections
* Ansible variables
* `register`
* Conditional task execution
* Secure secret handling
* Git feature branch workflow

---

## Sprint 1 – Ansible Project Foundation

### Added

* Created project directory structure.
* Initialized Git repository.
* Connected project to GitHub.
* Configured Ansible using `ansible.cfg`.
* Created static inventory with host groups.
* Added project `.gitignore`.
* Established repository structure for roles, playbooks, templates, variables, inventories, files, and documentation.

### Skills Practiced

* Git
* GitHub
* WSL
* Ansible installation
* Inventory management
* Project organization

