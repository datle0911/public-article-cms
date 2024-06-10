# Write-up
App Deployment using Microsoft Azure

## What Is Virtual Machine
Azure Infrastructure as a Service (IaaS) offers full access to the underlying operating system of a compute resource. These machines, available in Windows or Linux, offer high availability, scalability, and redundancy but require ongoing maintenance by developers.

## What Is App Service
Azure Platform as a Service (PaaS) allows developers to focus on apps rather than infrastructure. It hosts web applications, REST APIs, and mobile back ends, supporting multiple languages and continuous deployment.


## Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Appropriate solution
The appropriate solution for deploying this web application is App Service.

### Why I choose App Service
- **Cost:** Azure App Service is cost-effective compared to Virtual Machines due to various plan options and built-in load balancers.
- **Scalability:** Azure enables easy horizontal or vertical scaling, with Auto Scaling for automatic adjustments based on metrics.
- **Availability:** App Service ensures high availability with global hosting and an SLA guarantee.
- **Workflow:** App Service supports automated deployments from GitHub, Azure DevOps, or Git repositories.
- Azure App Service allows us to quickly build, deploy, and scale my web app.

### Why not Virtual Machines
- VMs require more setup and maintenance compared to the automated features of App Service.
- They offer full control but also increase responsibility for maintenance and security.


### Justification based on cost, scalability, availability, and workflow:

- **Cost:** Azure App Service is less expensive than Virtual Machines. It provides different plans options such as Free and Shared (preview) plans to test or deploy an app. App Services also have built-in load balancers that help save infrastructure costs.

- **Scalability:** Azure provides developers with the possibility to easily scale their apps either horizontally or vertically. Vertical scaling automatically increases or decreases resources allocated to our App Service, such as the amount of vCPUs or RAM, by changing the App Service pricing tier. Horizontal scaling increases or decreases the number of Virtual Machine instances our App Service is running.
    - With Auto scaling, App Service can automatically scale the number of instances based on a schedule or metrics like CPU, memory, or HTTP queue length. 

- **Availability:** Global scale with high availability. Using App Service, I can host my app anywhere in Microsoft's global datacenter infrastructure, and the App Service SLA promises high availability.

- **Workflow:** Azure App Service supports automated deployments from GitHub, Azure DevOps, or any Git repository. With GitHub Actions for Azure web app, developers can create workflows in GitHub repository to build, test, package, release, and deploy to Azure. 

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

- If the app expands significantly, VMs become more viable for their flexibility.
- Advanced scaling and traffic management may require VMs or specific Azure services.
- A change in the programming language might necessitate a different deployment approach.
- If server-level control or software installation is needed, VMs are the better option.
