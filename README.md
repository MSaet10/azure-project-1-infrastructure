# Azure Infrastructure Deployment Project

## Project Overview
This project demonstrates the deployment of a secure, scalable, and monitored Azure infrastructure environment. The environment includes virtual networking, virtual machines, load balancing, identity and access management, monitoring and alerting, serverless workflows, backup and disaster recovery, cost management, and incident simulation.

The goal of this project was to simulate a real-world Azure cloud environment and demonstrate cloud engineering, infrastructure deployment, monitoring, security, and operational troubleshooting skills.

## Technologies Used
- Microsoft Azure
- Azure Virtual Network (VNet)
- Azure Virtual Machines (Windows Server)
- Azure Load Balancer
- Network Security Groups (NSGs)
- Microsoft Entra ID
- Azure RBAC
- Azure Monitor
- Log Analytics Workspace
- Application Insights
- Azure Functions
- Azure Storage Account / Blob Storage
- Recovery Services Vault
- Azure Backup
- Azure Cost Management
- PowerShell
- Azure CLI
- Visual Studio Code

## Project Implementation

### Day 1 — Environment Setup
Set up the Azure environment by creating and validating the Azure subscription context, installing Azure CLI and local tools, creating the `rg-cloud-project` resource group, and applying tags for cost tracking and organization.

### Day 2 — Networking Layer
Built the networking foundation by creating the `vnet-cloud-project` virtual network with segmented subnets (`web-subnet` and `app-subnet`), creating Network Security Groups, adding inbound rules for HTTP, HTTPS, and restricted management access, and associating NSGs with subnets.

### Day 3 — Core Compute
Deployed Windows Server virtual machines in the web subnet, assigned public IPs for testing, connected through RDP, installed IIS, hosted a simple HTML web page, and validated web access over HTTP. Also configured a Windows container runtime and documented container troubleshooting.

### Day 4 — Load Balancer & High Availability
Created an Azure Standard Load Balancer, configured a frontend public IP, backend pool, HTTP health probe, and load balancing rule for port 80. Added both web VMs to the backend pool and tested failover by stopping one VM while confirming the application remained available through the load balancer. :contentReference[oaicite:0]{index=0}

### Day 5 — Identity & RBAC
Implemented identity and access control using Microsoft Entra ID by creating test users, assigning Reader and Contributor roles at the resource group scope, enabling MFA, and validating access restrictions through user testing. :contentReference[oaicite:1]{index=1}

### Day 6 — Monitoring & Observability
Configured Azure Monitor, Log Analytics Workspace, Azure Monitor Agent, Data Collection Rules, and alerting for high CPU, VM heartbeat loss, network traffic, and low disk space. Built a workbook dashboard for uptime, CPU, disk, and network monitoring. :contentReference[oaicite:2]{index=2}

### Day 7 — Serverless & Event-Driven Workflow
Created an Azure Storage Account, Blob container, and Azure Function App with a blob trigger. Developed and deployed the function from Visual Studio Code, then verified execution through uploaded files and Application Insights logs. :contentReference[oaicite:3]{index=3}

### Day 8 — Backup, Disaster Recovery & Cost Optimization
Created a Recovery Services Vault, enabled Azure Backup for virtual machines, generated recovery points, tested a VM restore, reviewed Azure Cost Management, and created monthly budget alerts for cost governance. :contentReference[oaicite:4]{index=4}

### Day 9 — Incident Simulation
Simulated real-world incidents including VM outage, NSG HTTP blocking, CPU spikes, low disk space, web service failure, and RBAC access denial. Verified that alerts fired correctly in Azure Monitor and Application Insights, then documented troubleshooting steps, resolutions, and lessons learned. 



