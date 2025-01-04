# Azure AKS MySQL Storage 💾🚀

## Overview 🌐

Welcome to the **Azure AKS MySQL Storage** project! This repository demonstrates how to leverage **Azure Disks** for persistent storage in **Azure Kubernetes Service (AKS)**, creating a MySQL database with a persistent volume claim (PVC) to ensure data durability. It also shows how to deploy a **User Management Web Application** with MySQL, managing configurations and connecting to the database seamlessly. 

The project covers:

- Creating **Azure Disk Storage** for AKS
- Deploying **MySQL** with persistence in Kubernetes
- Using **Kubernetes manifests** for storage classes, PVCs, and deployments
- Securing configurations with **Kubernetes ConfigMaps** and **Secrets** for sensitive data
- Creating a **User Management Web Application** that connects to the MySQL database

## 🚀 Features

- **Azure Disks**: Persistent storage for AKS applications
- **MySQL Database**: Managed via Kubernetes deployment and persistent storage
- **ConfigMaps**: Managing database schema and configurations
- **Secrets**: Securing sensitive information like database credentials
- **Kubernetes Manifests**: Easily deployable YAML files for all configurations
- **Web Application**: User management application that interacts with the MySQL database

## 🛠️ Technologies Used

- **Azure Kubernetes Service (AKS)** 🌐
- **Azure Disks** 💾
- **Kubernetes** 🛠️
- **MySQL** 🗃️
- **ConfigMaps & Secrets** 🔒
- **Helm (Optional)** 📦
- **kubectl** 🧑‍💻

## 🔑 Key Concepts

- **Persistent Volume Claim (PVC)**: Used to claim Azure Disk storage in AKS
- **Storage Class**: Determines the type of storage provisioned (e.g., managed-premium)
- **Deployment**: Pods running MySQL and the Web Application
- **ConfigMaps & Secrets**: Handling application configuration and sensitive data securely

## 📚 Documentation

Detailed steps are available in this repository to guide you through:

1. **Creating Azure Disks and PVCs**
2. **Deploying MySQL with persistent storage in AKS**
3. **Securing configurations with ConfigMaps & Secrets**
4. **Testing and interacting with the User Management Web Application**

---

## 📦 Getting Started

### Prerequisites

Before starting, make sure you have:

- A running **Azure Kubernetes Cluster (AKS)**
- **kubectl** configured to interact with your AKS cluster
- **Azure CLI** installed and logged in
- **MySQL Docker Image** (official or custom) 

---

Happy coding! 🚀
