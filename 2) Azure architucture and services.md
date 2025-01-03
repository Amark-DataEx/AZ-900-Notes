# Describe the core architectural components of Azure
This the module where we will learn about Azure physical organization : datacenters, availability zones and regions.
And also Azure organizational structure (management Infrastructure) : resources, resource groups and subscriptions.

## What is MS Azure?
Azure is a MS cloud computing platform with ever expanding services with help in your business expanstion.
Azure provides IaaS, PaaS, and SaaS.

Many teams start exploring the cloud by moving their existing applications to virtual machines (VMs) that run in Azure. Migrating your existing apps to VMs is a good start, but the cloud is much more than a different place to run your VMs.

For example, Azure provides artificial intelligence (AI) and machine-learning (ML) services that can naturally communicate with your users through vision, hearing, and speech. It also provides storage solutions that dynamically grow to accommodate massive amounts of data. Azure services enable solutions that aren't feasible without the power of the cloud.

## Get started with Azure accounts
* To create and use Azure services, you need an Azure subscription.
* When you're working with your own applications and business needs, you need to create an Azure account, and a subscription will be created for you.
* After you've created an Azure account, you're free to create additional subscriptions. For example, your company might use a single Azure account for your business and separate subscriptions for development, marketing, and sales departments.
* After you've created an Azure subscription, you can start creating Azure resources within each subscription.
[https://learn.microsoft.com/en-gb/training/wwl-azure/describe-core-architectural-components-of-azure/media/account-scope-levels-9ceb3abd-a2d45a13.png]
## Create an Azure account
You can create an azure account in three forms
* by signing up on the Azure website 
* through a Microsoft representative
* purchase Azure access through a Microsoft partner

## Core Architecture of Azure:
The core architectural components of Azure may be broken down into two main groupings: the physical infrastructure, and the management infrastructure.
## Physical Infrastructure:
Physical infrastructure starts with Azure datacenters.They’re facilities with resources arranged in racks, with dedicated power, cooling, and networking infrastructure.

Datacenters are grouped into Azure Regions or Azure Availability Zones that are designed to help you achieve resiliency and reliability for your business-critical workloads.
### Regions
A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network. Azure intelligently assigns and controls the resources within each region to ensure workloads are appropriately balanced.

When you deploy a resource in Azure, you'll often need to choose the region where you want your resource deployed.

     Some services or virtual machine (VM) features are only available in certain regions, such as specific VM sizes or storage types. There are also some global Azure services that don't require you to select a particular region, such as Microsoft Entra ID, Azure Traffic Manager, and Azure DNS.
### Availability Zones:
Availability zones are physically separate datacenters within an Azure region. Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking. An availability zone is set up to be an isolation boundary. If one zone goes down, the other continues working. Availability zones are connected through high-speed, private fiber-optic networks.

Availability zones are primarily for VMs, managed disks, load balancers, and SQL databases. Azure services that support availability zones fall into three categories:

* Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).
* Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).
* Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.

Even with the additional resiliency that availability zones provide, it’s possible that an event could be so large that it impacts multiple availability zones in a single region. To provide even further resilience, Azure has Region Pairs.
### Region Pairs:
Most Azure regions are paired with another region within the same geography (such as US, Europe, or Asia) at least 300 miles away. This approach allows for the replication of resources across a geography that helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region. For example, if a region in a pair was affected by a natural disaster, services would automatically fail over to the other region in its region pair.

