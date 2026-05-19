# 🚀 Terraform Phase

> **Infrastructure as Code (IaC)** project built using **Terraform** and **HCL** to automate cloud infrastructure provisioning and management.

This repository contains Terraform concepts, hands-on practice, reusable configurations, and real-world DevOps infrastructure examples — from basics to production-grade AWS and Kubernetes deployments.

---

## 📑 Table of Contents

- [Topics Covered](#-topics-covered)
- [Repository Structure](#-repository-structure)
- [Prerequisites](#-prerequisites)
- [Terraform Workflow](#-terraform-workflow)
- [Important Commands](#-important-terraform-commands)
- [Learning Goals](#-learning-goals)
- [Official Documentation](#-official-documentation)
- [Author](#-author)

---

## 📚 Topics Covered

### 🌱 Terraform Basics
- Introduction to Terraform
- Infrastructure as Code (IaC)
- Terraform Architecture
- Terraform Workflow
- Installing Terraform
- Terraform CLI Commands

---

### 🧱 HCL (HashiCorp Configuration Language)
- Syntax & Structure
- Types of Blocks
- Expressions & Functions
- String Interpolation
- Variables
- Outputs
- Local Variables (`locals`)

---

### ⚙️ Terraform Core Concepts

| Concept | Description |
|---|---|
| **Provider** | Plugins that interact with APIs (AWS, GCP, Azure) |
| **Resource** | Infrastructure components to be created/managed |
| **Variable** | Parameterized inputs for reusable configs |
| **Output** | Expose values after `apply` |
| **Module** | Reusable, encapsulated Terraform configurations |
| **State File** | Tracks real-world infrastructure state |
| **Lifecycle** | Controls create/update/destroy behavior |

---

### 🔁 Advanced Terraform
- Loops — `count`, `for_each`
- Conditional Expressions
- Dynamic Blocks
- Dependency Management (`depends_on`)
- State Manipulation (`terraform state`)
- Import Existing Infrastructure
- Terraform Graph
- Debugging Terraform Issues

---

### ☁️ AWS Infrastructure Automation

| Service | Purpose |
|---|---|
| **EC2** | Virtual compute instances |
| **VPC** | Isolated virtual networking |
| **Subnets** | Public & private subnet segmentation |
| **Internet Gateway** | Enable internet access for VPC |
| **Route Tables** | Traffic routing within VPC |
| **Security Groups** | Firewall rules for resources |
| **IAM Roles** | Permissions & access management |
| **S3 Buckets** | Object storage & remote state backend |

---

### ☸️ Kubernetes & DevOps
- Deploying EKS Cluster with Terraform
- Terraform with Kubernetes Provider
- CI/CD with Terraform
- Jenkins Integration
- Infrastructure Automation Pipelines

---

## 📂 Repository Structure

```bash
terraform-phase/
│
├── Basic-HCL/          # HCL syntax, blocks, expressions
├── Variables/          # Input variables, tfvars, validation
├── Outputs/            # Output values and references
├── Modules/            # Reusable module patterns
├── AWS/                # EC2, S3, IAM, Security Groups
├── VPC/                # Full VPC setup with subnets & routing
├── EKS/                # Kubernetes cluster on AWS EKS
├── CI-CD/              # Terraform in Jenkins pipelines
└── README.md
```

---

## 🛠️ Prerequisites

Before getting started, ensure you have a working knowledge of:

- 🐧 **Linux Basics** — command line, file system, permissions
- ☁️ **AWS Fundamentals** — services, IAM, console navigation
- 🔀 **Git & GitHub** — version control, branching, PRs
- 🌐 **Basic Networking** — IP, CIDR, subnets, routing
- 🐳 **Docker** — containerization concepts
- ☸️ **Kubernetes** — cluster architecture, pods, deployments

---

## ⚡ Terraform Workflow

```
📝 Write HCL Code
        ↓
terraform init        # Initialize providers & backend
        ↓
terraform validate    # Syntax & config validation
        ↓
terraform fmt         # Format code to standard style
        ↓
terraform plan        # Preview changes (dry run)
        ↓
terraform apply       # Provision infrastructure
        ↓
✅ Infrastructure Created
        ↓
terraform destroy     # Tear down when done
```

---

## 🚀 Important Terraform Commands

```bash
# Initialization
terraform init              # Download providers and modules

# Code Quality
terraform validate          # Check configuration validity
terraform fmt               # Auto-format HCL files

# Planning & Applying
terraform plan              # Show execution plan
terraform plan -out=tfplan  # Save plan to file
terraform apply             # Apply changes interactively
terraform apply -auto-approve  # Apply without confirmation

# State Management
terraform state list        # List all resources in state
terraform state show <resource>  # Show resource details
terraform state rm <resource>    # Remove resource from state

# Destruction
terraform destroy           # Destroy all managed infrastructure

# Utilities
terraform graph             # Generate dependency graph (use with Graphviz)
terraform output            # Show output values
terraform import            # Import existing infrastructure into state
```

---

## 🎯 Learning Goals

- [x] Understand Infrastructure as Code principles
- [x] Automate AWS infrastructure provisioning
- [x] Learn production-level Terraform patterns
- [x] Build and publish reusable modules
- [x] Integrate Terraform with CI/CD pipelines
- [x] Deploy Kubernetes (EKS) infrastructure via Terraform

---

## 📖 Official Documentation

| Resource | Link |
|---|---|
| 📘 Terraform Docs | [developer.hashicorp.com/terraform/docs](https://developer.hashicorp.com/terraform/docs) |
| ☁️ AWS Provider Docs | [registry.terraform.io/providers/hashicorp/aws](https://registry.terraform.io/providers/hashicorp/aws/latest/docs) |
| 📦 Terraform Registry | [registry.terraform.io](https://registry.terraform.io/) |
| ☸️ Kubernetes Provider | [registry.terraform.io/providers/hashicorp/kubernetes](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs) |

---

## 👨‍💻 Author

**Suman Ranjan**
*DevOps & Cloud Enthusiast 🚀*

[![GitHub](https://img.shields.io/badge/GitHub-SumnRanjan-181717?style=for-the-badge&logo=github)](https://github.com/SumnRanjan)

---

<div align="center">

⭐ **Star this repo if it helped you on your DevOps journey!** ⭐

*Built with 💙 using Terraform | HashiCorp | AWS | Kubernetes*

</div>