# 🚀 Ansible Playbook for Installing Docker and Jenkins

This Ansible playbook automates the installation of **Docker** and **Jenkins** on both **Ubuntu** and **RedHat-based** systems.

---

## 📌 Requirements

### 🔹 Control Node:
- Ansible installed (`ansible` command available).
- SSH access to the target machines.

### 🔹 Managed Nodes (Target Machines):
- **OS:** Ubuntu or RedHat-based distributions (CentOS, RHEL, Rocky Linux).
- Sudo privileges enabled.

---

## 📂 Project Structure

```plaintext
ansible/
│── ansible.cfg         # Ansible configuration file
│── inventory           # List of target hosts
│── main.yml            # Main playbook file
└── roles/              # Role-based structure
    ├── docker/         # Docker installation role
    │   ├── tasks/      # Tasks for installing Docker
    │   ├── handlers/   # Handlers for Docker service
    │   ├── defaults/   # Default variables
    │   └── README.md   # Role-specific documentation
    └── jenkins/        # Jenkins installation role
        ├── tasks/      # Tasks for installing Jenkins
        ├── handlers/   # Handlers for Jenkins service
        ├── defaults/   # Default variables
        └── README.md   # Role-specific documentation
