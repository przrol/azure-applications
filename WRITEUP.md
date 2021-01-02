# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*

    |  | App Service | Virtual machine |
    | ------------ | ------------ | ------------ |
    | *Scalability* | up to 14 GB memory and 4 CPUs | no limit; Virtual Machine Scale Sets and Load Balancers |
    | *Costs*   | always paying for the service plan | more expensive      |
    | *Availability*   | high availability | high availability     |
    | *Workflow*   | limited access to the host server |  full access and control of the VM   |

- *Choose the appropriate solution (VM or App Service) for deploying the app*
    - I deploy the app as an App Service
- *Justify your choice*
    - The app is a lightweight solution
    - App Services are more expensive than VMs but easier to handle

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*

I would choose a VM if:
- Requirements greater than 14 GB memory and 4 CPUs
- Another language is necessary than .NET, .NET Core, Java, Ruby, Node.js, PHP, or Python
- Need to control the underlying OS (i.e. software installation)
- Need to install custom images
- Migrating from an on-premises server to the cloud