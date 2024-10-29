# Ansible Development Environment Setup

This project uses Ansible to automate the setup of a local development environment with organized roles for flexibility and cross-distro compatibility. It ensures that all required folders, dependencies, and repositories are set up consistently on any Linux distribution.

## Table of Contents

- [Folder Structure](#folder-structure)
- [License](#license)

---

## Folder Structure

```plaintext
network-setup-engine/
├── setup-dev.yml               # Main playbook
├── inventory.ini               # Inventory file
├── roles/                      # Roles directory
│   └── ansible-network-dev/                 # Role for common setup tasks
│       ├── meta/                        # Includes all meta info of this role
│       │   ├── main.yml
│       ├── tasks/
│       │   ├── main.yml                # Includes all tasks for this role
│       │   ├── create_dirs.yml         # Task file for creating required git directories
│       │   └── clone_basic_repos.yml   # Task file for cloning basic required git repositories
│       │   └── clone_cisco_repos.yml   # Task file for cloning cisco related Git repositories
│       └── vars/
│           └── main.yml         # Default variables for common role
└── README.md                   # Documentation for the project
```

## License

This project is licensed under the MIT License.
