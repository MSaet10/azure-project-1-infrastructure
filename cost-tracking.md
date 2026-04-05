# Cost Tracking and Optimization — Azure Project

## Cost Management Overview
Azure Cost Management was used to monitor resource costs, analyze spending by resource, and create budget alerts to prevent overspending.

## Resources Generating Cost
The main Azure resources generating cost in this project included:

- Virtual Machines
- Managed Disks
- Public IP Addresses
- Azure Load Balancer
- Log Analytics Workspace
- Storage Account
- Azure Functions (Consumption plan)
- Recovery Services Vault (Backup storage)

## Cost Optimization Steps Implemented
The following cost optimization strategies were implemented:

- Stopped (deallocated) virtual machines when not in use
- Used Standard HDD managed disks instead of Premium SSD
- Used Consumption plan for Azure Functions (serverless pricing)
- Created budget alerts to monitor spending
- Tagged resources for cost tracking using the tag:
  - Project: CloudPortfolio
- Reviewed Cost Analysis by resource to identify highest cost services

## Budget Alerts
A monthly budget was created with alerts at:
- 50% budget usage
- 70% budget usage
- 80% budget usage

This helps prevent unexpected Azure charges.

## Cost Monitoring Tools Used
- Azure Cost Management
- Cost Analysis
- Azure Budgets
- Resource Tags
- Azure Advisor (cost recommendations)

## Cost Management Lessons Learned
- Virtual Machines are typically the largest cost in Azure environments.
- Log Analytics can become expensive depending on data ingestion.
- Backup storage in Recovery Services Vault adds storage cost.
- Public IPs and Load Balancers also contribute to monthly cost.
- Stopping unused resources significantly reduces cost.
- Budget alerts are important for cost governance.
