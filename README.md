## Resources: 
Resources are instances of services that you create, like virtual machines, storage, or SQL databases.   

## Resource groups: 
Resources are combined into resource groups, which act as a logical container into which Azure resources like web apps, databases, and storage accounts are deployed and managed.   

## Subscriptions: 
A subscription groups together user accounts and the resources that have been created by those user accounts. For each subscription, there are limits or quotas on the amount of resources that you can create and use. Organizations can use subscriptions to manage costs and the resources that are created by users, teams, or projects. 

## Management groups:
These groups help you manage access, policy, and compliance for multiple subscriptions. All subscriptions in a management group management group. automatically inherit the conditions applied to the management Group.

<img src="./images/resources_group.png" width=40% height=40%/>   


# Resource Groups  
`Resources:` are anything you create in an Azure subscription like VMs, Azure Application Gateway instances, and Azure Cosmos DB instances.   
* Resource group is a logical container which help manage and organize your Azure resources.   
For example imilar usage, type, or location   
* Each resource can exist in only one resource group.
* You can move a resource from one resource group to another group.  
* Resource groups can't be nested.   
* The resources in a resource group can be located in different regions than the resource group.   
* Resource group created at location to store metadata.    
* A resource group can be used to scope access control for administrative actions. To manage a resource group, you can assign Azure Policies, Azure roles, or resource locks.  
   * You can apply locks to a resource group or subscription to prevent deletion or make contained resources read-only. You can also apply locks directly to a resource.  
* You can apply tags to a resource group. The resources in the resource group don't inherit those tags.   
* Life cycle: When you delete a resource group, all resources in the resource group are also deleted.   
* To create a resource group, you can use the portal, PowerShell, Azure CLI, or an ARM template.   


 
# AZURE RESOURCE MANAGER(ARM)

Azure Resource Manager is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account.   
When you send a request through any of the Azure APIs, tools, or SDKs, Resource Manager receives the request. It authenticates and authorizes the request before forwarding it to the appropriate Azure service.      

<img src="./images/arm.png" width=60% height=60%/> 

* Atomate resource deployments (create, update, and delete) using templates.   
* ARM template is a JSON file that defines what you want to deploy to Azure.   
* Integrates with Azure portal, PowerShell, CLI, and REST API to perform deployment and management tasks.   
* Easy way to deploy multiple resource instances or reliably redeploy resources.  
* ARM template can be used to deploy the resources consistently and repeatedly.  
* Define the dependencies between resources so they're deployed in the correct order.   

<img src="./images/rg_template.png" width=60% height=60%/>


