# Lessons Learned — Azure Infrastructure Project

## Networking
- Virtual Networks allow segmentation of cloud environments.
- Subnets separate application tiers (web tier and app tier).
- Network Security Groups act as firewalls controlling inbound and outbound traffic.
- NSG rules have priorities and can block traffic if misconfigured.
- NIC-level NSGs override subnet NSGs.

## Compute
- Azure Virtual Machines can host web applications using IIS.
- Public IPs allow external access but should be restricted for security.
- VM sizing and disk types affect cost and performance.
- Stopping (deallocating) VMs reduces compute costs.

## Load Balancer & High Availability
- Azure Load Balancer distributes traffic across multiple backend VMs.
- Health probes determine which backend instances are healthy.
- High availability requires at least two backend virtual machines.
- Failover testing is important to validate high availability.

## Identity & RBAC
- Microsoft Entra ID manages users and authentication.
- Azure RBAC controls access using roles such as Reader and Contributor.
- RBAC roles can be assigned at subscription, resource group, or resource level.
- Multi-factor authentication improves cloud security.
- Reader users cannot modify resources and are blocked by Azure RBAC.

## Monitoring & Observability
- Azure Monitor provides metrics and alerts.
- Log Analytics stores logs and performance data.
- Azure Monitor Agent collects telemetry from virtual machines.
- Data Collection Rules define what logs and metrics are collected.
- Alerts can be created for CPU usage, disk space, network traffic, and VM availability.
- Workbooks provide dashboards for monitoring infrastructure.

## Serverless & Event-Driven Architecture
- Azure Functions provide serverless compute.
- Blob Storage triggers allow event-driven workflows.
- Application Insights stores function execution logs.
- Serverless reduces infrastructure management and cost.

## Backup & Disaster Recovery
- Recovery Services Vault stores backups and recovery points.
- Backup policies control backup frequency and retention.
- Restoring a VM from backup verifies disaster recovery capability.
- Backup and restore testing is important for real-world environments.

## Cost Management
- Azure Cost Management tracks resource costs.
- Budget alerts help prevent overspending.
- Virtual machines, disks, and Log Analytics are major cost contributors.
- Stopping unused resources reduces cost.

## Incident Simulation & Troubleshooting
- Monitoring alerts detect outages and performance issues.
- NSG rules can cause application outages if misconfigured.
- High CPU and low disk space alerts help detect performance problems.
- Application Insights availability tests detect application failures.
- RBAC prevents unauthorized changes to resources.

## Overall Project Lessons
This project demonstrated how to design, deploy, monitor, secure, and maintain a cloud infrastructure environment in Microsoft Azure. It also demonstrated troubleshooting, incident response, backup and recovery, cost management, and documentation practices used in real-world cloud environments.