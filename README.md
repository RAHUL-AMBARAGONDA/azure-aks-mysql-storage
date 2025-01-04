# **Azure AKS Storage with Azure Disks - Project Overview**

## **Introduction**

Welcome to the **Azure AKS Storage with Azure Disks** project! This project demonstrates how to deploy a MySQL database with persistent storage using **Azure Disks** in **Azure Kubernetes Service (AKS)**. Along with deploying a MySQL database, we also integrate a **User Management Web Application** that connects to the database for managing users.

This project leverages **Kubernetes Persistent Volumes (PV)** and **Persistent Volume Claims (PVC)** for managing storage within AKS, ensuring data persistence across container restarts. Additionally, we explore advanced Kubernetes features such as **ConfigMaps**, **Secrets**, **LoadBalancer services**, and **Azure Disk storage classes** to create a production-grade solution.

---

## **What’s Covered**

- **Storage Configuration**: How to configure Azure Disks with Kubernetes for persistent storage.
- **MySQL Database**: Deploying a MySQL database with persistent storage.
- **Web Application**: Deploying a user management web application connected to MySQL.
- **Secrets and ConfigMaps**: Securely managing sensitive information like database passwords and configurations.
- **Advanced Features**: Using Azure Disk storage classes, LoadBalancers, and persistent volumes.
- **Cost Optimization**: Best practices for selecting storage classes and optimizing costs in a production environment.

---

## **Key Concepts and Technologies Used**

- **Azure Kubernetes Service (AKS)**
- **Azure Disks** (Persistent Storage)
- **Persistent Volumes (PV)** and **Persistent Volume Claims (PVC)**
- **ConfigMaps** and **Secrets** for configuration management
- **MySQL Database** on Kubernetes
- **Kubernetes Deployments**, **Services**, and **LoadBalancers**
- **Azure Storage Classes** and **Cost Optimization** Techniques

---

## **Project Setup**

1. **Create an AKS Cluster**: Ensure you have an AKS cluster set up and kubectl configured.
2. **Azure Resources**: Have access to Azure for managing resources like Disks and Storage Classes.
3. **Kubernetes Tools**: Familiarity with kubectl and YAML-based Kubernetes object management.

---

## **Folder Structure**

The project folder structure is as follows:

```
.
├── kube-manifests
│   ├── 01-storage-class.yml
│   ├── 02-persistent-volume-claim.yml
│   ├── 03-usermgmt-configmap.yml
│   ├── 04-mysql-deployment.yml
│   ├── 05-mysql-clusterip-service.yml
│   ├── 06-usermgmt-webapp-deployment.yml
│   ├── 07-usermgmt-webapp-service.yml
│   ├── secrets
│   │   └── mysql-secrets.yml
└── README.md
```

---

## **Getting Started**

### **Prerequisites**

Before you begin, ensure you have the following prerequisites:

1. **Azure Account** with access to AKS and Disk Management.
2. **Kubectl** CLI installed and configured for accessing your AKS cluster.
3. A basic understanding of **Kubernetes** objects such as Deployments, Services, and Secrets.
4. **MySQL** image knowledge, as we will deploy MySQL inside Kubernetes.

### **Setup Instructions**

1. Clone this repository to your local machine or fork it to your own GitHub account.
2. Apply the Kubernetes manifests located in the `kube-manifests` directory to your AKS cluster.
3. Follow the step-by-step guide outlined in the README to deploy the MySQL database and the User Management Web Application.

---

## **Next Steps**

1. **Deploying Resources**: Apply the Kubernetes manifests to create persistent volumes, deploy MySQL, and set up your web application.
2. **Accessing Services**: Use the LoadBalancer service to access the user management web application from outside the cluster.
3. **Testing**: Create users, interact with the database, and verify persistent storage across pod restarts.

---

## **Conclusion**

This project serves as an excellent starting point for setting up persistent storage in AKS, deploying stateful applications like MySQL, and integrating advanced Kubernetes features. By following the steps in this guide, you'll not only learn how to use Azure Disks in AKS but also how to securely manage configurations, scale applications, and optimize resources for production use.

For more advanced usage and customization, refer to the individual YAML files in the `kube-manifests` directory.

--- 

Feel free to contribute and customize the project to meet your specific requirements.
