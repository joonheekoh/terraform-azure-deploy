# Terraform Azure VM Deployment

This repository contains Infrastructure-as-Code (IaC) for provisioning a Virtual Machine and its required networking resources on **Microsoft Azure** using **Terraform**. The VM is used as the deployment target for multiple containerised Node.js applications hosted under `joonheedevops.com`.

---

## 📁 Project Structure

### 📁 Project Structure

```plaintext
terraform-azure-deploy/
├── .gitignore         # Git ignore rules to avoid committing sensitive or large files
├── README.md          # Project documentation
├── main.tf            # Main Terraform configuration for Azure resources
├── cloud-init.yaml    # Cloud-init script for provisioning the Linux VM
├── azure_vm_key       # Private SSH key (should NOT be committed)
├── azure_vm_key.pub   # Public SSH key used by the VM
└── .terraform/        # Terraform provider plugins (excluded via .gitignore)