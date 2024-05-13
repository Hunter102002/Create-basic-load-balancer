# Create a basic load balancer

## Objective

The Basic Load Balancer Configuration project involved setting up a load balancer in Azure to distribute network traffic across multiple servers, enhancing the application's availability and reliability. The main objective was to ensure efficient handling of incoming network traffic and improve fault tolerance within the server environment.

### Skills Learned

- Load Balancer Setup: Configured Azure's Load Balancer to distribute incoming network traffic evenly among multiple VMs, ensuring no single server becomes a bottleneck.
- Health Probes Configuration: Implemented health probes to monitor the status of VMs, allowing the load balancer to redirect traffic away from failing or underperforming servers.
- Backend Pools Management: Organized VMs into backend pools for efficient management and traffic distribution, ensuring that workloads are evenly distributed across available servers.
- Fault Tolerance and Redundancy: Enhanced system resilience and reliability by setting up redundant instances to handle potential server failures without service interruption.

### Tools Used

- Azure Portal and Azure CLI: Utilized for configuring and managing the load balancer settings.
- Azure PowerShell: Employed for automating the setup and configuration tasks.
- Network Monitoring Tools: Used for real-time monitoring of network traffic and performance metrics to optimize load balancing rules.
- Azure Resource Manager (ARM) Templates: Leveraged for deploying consistent and repeatable configurations across multiple environments.

## Steps
Create a virtual network with a new subnet![Screenshot 2024-05-13 at 11 03 48 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/cb6bbca8-a9fe-4325-a780-0c36c172039c)

Verify VNET![Screenshot 2024-05-13 at 11 04 24 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/d6d08d89-30ec-449c-b9f2-00b02491ede4)



Create Availability set

![Screenshot 2024-05-13 at 11 05 35 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/4454022b-a5a6-48c1-8c70-7b4c68dd4b62)

Create 2 VMs![Screenshot 2024-05-13 at 11 10 57 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/0999344e-1c4f-4285-92a4-9bdabf9b8734)

Sign into on prem machine and assign roles![Screenshot 2024-05-13 at 11 19 47 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/178aefd9-b2eb-4740-ad5f-b68d1f06808f)



Verify installation 

![Screenshot 2024-05-13 at 11 31 02 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/05bd61ea-2a4b-4846-8c6a-8142eb8fd643)


Add Frontend Config in Load balancer

![Screenshot 2024-05-13 at 11 34 15 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/4b8461f8-19f6-4f0b-bf3c-4171be81b4ea)

Add Backend pool in load balancer


![Screenshot 2024-05-13 at 11 35 07 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/68265a1c-e4ef-4b1d-8cfe-d296f1c9e21f)

Add Load balancing rule 


![Screenshot 2024-05-13 at 11 36 33 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/309071dc-0933-45a2-87ac-8a0d57afc46e)

Verify Load balancer![Screenshot 2024-05-13 at 11 38 32 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/0ff9e1a8-e86b-49c5-b49d-a41a921add56)

Verify IP address

![Screenshot 2024-05-13 at 11 40 48 AM](https://github.com/Hunter102002/Create-basic-load-balancer/assets/98543129/d4258aa2-effa-49c7-a90c-2981befecbb0)
