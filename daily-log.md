# Daily Project Log — Azure Infrastructure Project

## Day 1 — Environment Setup
Created Azure subscription environment, installed Azure CLI, Visual Studio Code, and PowerShell modules. Created resource group rg-cloud-project and applied resource tags for cost tracking.

## Day 2 — Networking Layer
Created virtual network vnet-cloud-project with address space 10.0.0.0/16. Created web-subnet and app-subnet. Created Network Security Groups and configured inbound rules for HTTP, HTTPS, and RDP. Associated NSGs with subnets.

## Day 3 — Core Compute
Deployed Windows virtual machines in web-subnet. Connected using RDP. Installed IIS web server and hosted a simple HTML web page. Verified web server access through public IP.

## Day 4 — Load Balancer & High Availability
Created Azure Load Balancer with frontend public IP. Configured backend pool, health probe, and load balancing rule. Added both VMs to backend pool and tested failover by stopping one VM.

## Day 5 — Identity & RBAC
Created test users in Microsoft Entra ID. Assigned Reader and Contributor roles at resource group scope. Enabled multi-factor authentication and tested access restrictions.

## Day 6 — Monitoring & Observability
Created Log Analytics Workspace. Installed Azure Monitor Agent and configured Data Collection Rules. Created alerts for CPU usage, VM heartbeat, network traffic, and disk space. Built Azure Monitor Workbook dashboard.

## Day 7 — Serverless & Event-Driven Workflow
Created Azure Storage Account and Blob container. Created Azure Function App with blob trigger. Deployed function from Visual Studio Code and verified execution using Application Insights logs.

## Day 8 — Backup, Disaster Recovery & Cost Optimization
Created Recovery Services Vault. Enabled Azure Backup for virtual machines. Ran backups and performed VM restore test. Reviewed Azure Cost Management and created budget alerts.

## Day 9 — Incident Simulation
Simulated VM outage, NSG blocking HTTP, high CPU usage, low disk space, web server failure, and RBAC access denial. Verified alerts triggered and documented troubleshooting steps.

## Day 10 — Documentation & GitHub
Created architecture diagram, organized screenshots, completed documentation files, and uploaded project to GitHub repository.