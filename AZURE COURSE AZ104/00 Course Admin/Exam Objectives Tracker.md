---
course: AZ-104
title: Exam Objectives Tracker
type: admin
updated: 2026-09-17
tags:
  - az104
  - admin
  - revision
---

# AZ-104 Exam Objectives Tracker

The official skills-measured list, with the module that covers each area. Ticks are synced from the module notes as of **17 September 2026**.

Tick things off as you get confident, not as you sit through them. The test is whether you could do it in the portal unaided.

**Index:** [[AZ-104 Course Index]]

---

## Coverage at a glance

| Domain | Weight | Done | Total |
| --- | :--: | :--: | :--: |
| Manage Azure identities and governance | 20-25% | **15** | 15 |
| Implement and manage storage | 15-20% | **16** | 17 |
| Deploy and manage Azure compute resources | 20-25% | **17** | 24 |
| Implement and manage virtual networking | 15-20% | **11** | 13 |
| Monitor and maintain Azure resources | 10-15% | **13** | 13 |
| **Total** | | **72** | **82** |

---

## Manage Azure identities and governance — 20-25%

### Manage Microsoft Entra users and groups — [[01 - Administer Identity]]

- [x] Create users and groups
- [x] Manage user and group properties
- [x] Manage licences in Microsoft Entra ID
- [x] Manage external users
- [x] Configure self-service password reset (SSPR)

### Manage access to Azure resources — [[02 - Governance and Compliance]]

- [x] Manage built-in Azure roles
- [x] Assign roles at different scopes
- [x] Interpret access assignments

### Manage Azure subscriptions and governance — [[02 - Governance and Compliance]]

- [x] Implement and manage Azure Policy
- [x] Configure resource locks
- [x] Apply and manage tags on resources
- [x] Manage resource groups
- [x] Manage subscriptions
- [x] Manage costs by using alerts, budgets and Azure Advisor recommendations
- [x] Configure management groups

---

## Implement and manage storage — 15-20%

### Configure access to storage — [[07 - Azure Storage]]

- [x] Configure Azure Storage firewalls and virtual networks
- [x] Create and use shared access signature (SAS) tokens
- [x] Configure stored access policies
- [x] Manage access keys
- [x] Configure identity-based access for Azure Files

### Configure and manage storage accounts — [[07 - Azure Storage]]

- [x] Create and configure storage accounts
- [x] Configure Azure Storage redundancy
- [x] Configure object replication
- [x] Configure storage account encryption
- [x] Manage data by using Azure Storage Explorer and AzCopy

### Configure Azure Files and Azure Blob Storage — [[07 - Azure Storage]]

- [x] Create and configure a file share in Azure Files
- [x] Create and configure a container in Azure Blob Storage
- [x] Configure storage tiers
- [x] Configure soft delete for blobs and containers
- [x] Configure snapshots and soft delete for Azure Files
- [x] Configure blob lifecycle management
- [ ] Configure blob versioning

---

## Deploy and manage Azure compute resources — 20-25%

### Automate deployment with ARM templates or Bicep — [[03 - Administer Azure Resources]]

> Note is written up; objectives left unticked until the lab is done hands-on.

- [ ] Interpret an ARM template or a Bicep file
- [ ] Modify an existing ARM template
- [ ] Modify an existing Bicep file
- [ ] Deploy resources by using an ARM template or a Bicep file
- [ ] Export a deployment as an ARM template, or convert ARM JSON to Bicep

### Create and configure virtual machines — [[08 - Azure Virtual Machines]]

- [x] Create a virtual machine
- [x] Configure encryption at host
- [x] Manage virtual machine sizes
- [x] Manage virtual machine disks
- [x] Deploy VMs to availability zones and availability sets
- [x] Deploy and configure Azure Virtual Machine Scale Sets
- [ ] Move a VM to another resource group, subscription or region

### Provision and manage containers — [[09 - PaaS Compute Options]]

- [x] Create and manage an Azure Container Registry
- [x] Provision a container by using Azure Container Instances
- [x] Provision a container by using Azure Container Apps
- [x] Manage sizing and scaling for containers

### Create and configure Azure App Service — [[09 - PaaS Compute Options]]

- [x] Provision an App Service plan
- [x] Configure scaling for an App Service plan
- [x] Create an App Service
- [x] Configure certificates and TLS for an App Service
- [x] Map an existing custom DNS name to an App Service
- [ ] Configure backup for an App Service
- [x] Configure networking settings for an App Service
- [x] Configure deployment slots for an App Service

---

## Implement and manage virtual networking — 15-20%

### Configure and manage virtual networks — [[04 - Virtual Networking]] / [[05 - Intersite Connectivity]]

- [x] Create and configure virtual networks and subnets
- [x] Create and configure virtual network peering
- [x] Configure public IP addresses
- [x] Configure user-defined routes
- [x] Troubleshoot network connectivity

### Configure secure access to virtual networks — [[04 - Virtual Networking]]

- [x] Create and configure NSGs and application security groups
- [x] Evaluate effective security rules in NSGs
- [x] Implement Azure Bastion
- [ ] Configure service endpoints for Azure PaaS
- [ ] Configure private endpoints for Azure PaaS

### Configure name resolution and load balancing — [[06 - Network Traffic Management]]

- [x] Configure Azure DNS
- [x] Configure an internal or public load balancer
- [x] Troubleshoot load balancing

---

## Monitor and maintain Azure resources — 10-15%

### Monitor resources in Azure — [[11 - Monitoring]]

- [x] Interpret metrics in Azure Monitor
- [x] Configure log settings in Azure Monitor
- [x] Query and analyse logs in Azure Monitor
- [x] Set up alert rules, action groups and alert processing rules
- [x] Configure and interpret VM, storage and network Insights
- [x] Use Azure Network Watcher and Connection monitor

### Implement backup and recovery — [[10 - Data Protection]]

- [x] Create a Recovery Services vault
- [x] Create an Azure Backup vault
- [x] Create and configure a backup policy
- [x] Perform backup and restore operations by using Azure Backup
- [x] Configure Azure Site Recovery for Azure resources
- [x] Perform a failover to a secondary region by using Site Recovery
- [x] Configure and interpret reports and alerts for backups

---

## What's left, in priority order

All eleven module notes are written. Everything below is either a genuine gap in the notes or something that only counts once it's been done hands-on.

| | Area | Why |
| :-- | --- | --- |
| **1** | **ARM / Bicep hands-on — [[03 - Administer Azure Resources]]** | Note is written; the objectives stay unticked until [[LAB 03 - Manage Azure Resources with ARM Templates]] is done unaided |
| **2** | **Service and private endpoints — [[04 - Virtual Networking]]** | The two loose ends in networking, and a favourite exam scenario |
| **3** | **Blob versioning — [[07 - Azure Storage]]** | The one storage objective not covered; easy win |
| **4** | **App Service backup — [[09 - PaaS Compute Options]]** | The one App Service objective not covered |
| **5** | **Moving a VM between resource groups, subscriptions or regions — [[08 - Azure Virtual Machines]]** | Not covered in the module note |
| **6** | **Recall checks across all 11 modules** | The real test of whether any of this has stuck |

---

**Source:** [AZ-104 study guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-104)
