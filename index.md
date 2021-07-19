---
title: Online Hosted Instructions
permalink: index.html
layout: home
---
# Course AZ-104T00: Microsoft Azure Administrator

This course teaches IT Professionals how to manage their Azure subscriptions, secure identities, administer the infrastructure, configure virtual networking, connect Azure and on-premises sites, manage network traffic, implement storage solutions, create and scale virtual machines, implement web apps and containers, back up and share data, and monitor your solution.

### Audience Profile
This course is for Azure Administrators. The Azure Administrator implements, manages, and monitors identity, governance, storage, compute, and virtual networks in a cloud environment. The Azure Administrator will provision, size, monitor, and adjust resources as appropriate.

### Prerequisites
Successful Azure Administrators start this role with experience in virtualization, networking, identity, and storage.

Understanding of on-premises virtualization technologies, including: VMs, virtual networking,
and virtual hard disks.

Understanding of network configurations, including TCP/IP, Domain Name System (DNS),
virtual private networks (VPNs), firewalls, and encryption technologies.

Understanding of Active Directory concepts, including users, groups, and role-based access
control.

Understanding of resilience and disaster recovery, including backup and restore operations.

### Course outline
### Module 1: Identity
In this module, you will learn how to secure identities with Azure Active Directory, and implement users and groups.

#### Lessons

* Azure Active Directory
* Users and Groups

### Lab : Manage Azure Active Directory Identities
After completing this module, students will be able to:

* Secure and manage identities with Azure Active Directory.
* Implement and manage users and groups.

### Module 2: Governance and Compliance
In this module, you will learn about managing your subscriptions and accounts, implementing Azure policies, and using Role-Based Access Control.

### Lessons

* Subscriptions and Accounts
* Azure Policy

### Role-based Access Control (RBAC)

* Lab : Manage Subscriptions and RBAC
* Lab : Manage Governance via Azure Policy

After completing this module, students will be able to:

* Implement and manage Azure subscriptions and accounts.
* Implement Azure Policy, including custom policies.
* Use RBAC to assign permissions.

### Module 3: Azure Administration
In this module, you will learn about the tools an Azure Administrator uses to manage their infrastructure. This includes the Azure Portal, Cloud Shell, Azure PowerShell, CLI, and Resource Manager Templates. This module includes:

### Lessons

* Azure Resource Manager
* Azure Administrator Tools
* ARM Templates

* Lab : Manage Azure resources by Using ARM Templates
* Lab : Manage Azure resources by Using Azure PowerShell (optional)
* Lab : Manage Azure resources by Using Azure CLI (optional)
* Lab : Manage Azure resources by Using the Azure Portal

After completing this module, students will be able to:

* Leverage Azure Resource Manager to organize resources.
* Use the Azure Portal and Cloud Shell.
* Use Azure PowerShell and CLI.
* Use ARM Templates to deploy resources.

### Module 4: Virtual Networking
In this module, you will learn about basic virtual networking concepts like virtual networks and subnetting, IP addressing, network security groups, Azure Firewall, and Azure DNS.

### Lessons

* Virtual Networks
* Network Security groups
* Azure Firewall
* Azure DNS

*Lab : Implement Virtual Networking

After completing this module, students will be able to:

* Implement virtual networks and subnets.
* Configure network security groups.
* Configure Azure Firewall.
* Configure private and public DNS zones.

### Module 5: Intersite Connectivity
In this module, you will learn about intersite connectivity features including VNet Peering, Virtual Network Gateways, and Site-to-Site Connections.

### Lessons

* VNet Peering
* VPN Gateway Connections
* ExpressRoute and Virtual WAN

* Lab : Implement Intersite Connectivity

After completing this module, students will be able to:

* Configure VNet Peering.
* Configure VPN gateways.
* Choose the appropriate intersite connectivity solution.

### Module 6: Network Traffic Management
In this module, you will learn about network traffic strategies including network routing and service endpoints, Azure Load Balancer, and Azure Application Gateway.

### Lessons

* Network Routing and Endpoints
* Azure Load Balancer
* Azure Application Gateway

Lab : Implement Traffic Management

After completing this module, students will be able to:

* Configure network routing including custom routes and service endpoints.
* Configure an Azure Load Balancer.
* Configure and Azure Application Gateway.

### Module 7: Azure Storage
In this module, you will learn about basic storage features including storage accounts, blob storage, Azure files and File Sync, storage security, and storage tools.

### Lessons

* Storage Accounts
* Blob Storage
* Storage Security
* Azure Files and File Sync
* Managing Storage

### Lab : Manage Azure storage

* After completing this module, students will be able to:
* Create Azure storage accounts.
* Configure blob containers.
* Secure Azure storage.
* Configure Azure files shares and file sync.
* Manage storage with tools such as Storage Explorer.

### Module 8: Azure Virtual Machines
In this module, you will learn about Azure virtual machines including planning, creating, availability and extensions.

### Lessons

* Virtual Machine Planning
* Creating Virtual Machines
* Virtual Machine Availability
* Virtual Machine Extensions

### Lab : Manage virtual machines

After completing this module, students will be able to:

* Plan for virtual machine implementations.
* Create virtual machines.
* Configure virtual machine availability, including scale sets.
* Use virtual machine extensions.

### Module 9: Serverless Computing
In this module, you will learn how to administer serverless computing features like Azure App Service, Azure Container Instances, and Kubernetes.

### Lessons

* Azure App Service Plans
* Azure App Service
* Container Services
* Azure Kubernetes Service

Lab : Implement Web Apps
Lab : Implement Azure Kubernetes Service
Lab : Implement Azure Container Instances

After completing this module, students will be able to:

* Create an app service plan.
* Create a web app.
* Implement Azure Container Instances.
* Implement Azure Kubernetes Service.

### Module 10: Data Protection

In this module, you will learn about backing up files and folders, and virtual machine backups.

### Lessons

* File and Folder Backups
* Virtual Machine Backups

### Lab : Implement Data Protection

After completing this module, students will be able to:

* Backup and restore file and folders.
* Backup and restore virtual machines.

### Module 11: Monitoring
In this module, you will learn about monitoring your Azure infrastructure including Azure Monitor, alerting, and log analytics.

### Lessons

* Azure Monitor
* Azure Alerts
* Log Analytics
* Network Watcher

### Lab : Implement Monitoring

After completing this module, students will be able to:

* Use Azure Monitor.
* Create Azure alerts.
* Query using Log Analytics.
* Use Network Watcher.

---

Required labs files can be [DOWNLOADED HERE](https://github.com/AceTheCloud/AZ-104.github.io/archive/master.zip)

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Module | Lab |
| --- | --- |
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

All Labs Prepared by Microsoft and Microsoft Learn Community
