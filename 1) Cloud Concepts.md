# Azure Fundamentals
* Microsoft Azure is a cloud computing platform with an ever-expanding set of services to help you build solutions to meet your business goals. 
* Azure services support everything from simple to complex. 
* Azure has simple web services for hosting your business presence in the cloud. Azure also supports running fully virtualized computers managing your custom software solutions. Azure provides a wealth of cloud-based services like remote storage, database hosting, and centralized account management. Azure also offers new capabilities like artificial intelligence (AI) and Internet of Things (IoT) focused services.
* ``` Whether you're interested in compute, networking, or storage services; learning about cloud security best practices; or exploring governance and management options, think of Azure Fundamentals as your curated guide to Azure.```

AZ-900: Microsoft Azure Fundamentals. This exam includes three knowledge domain areas:

1. Describe cloud concepts 
2. Describe Azure architecture and services	
3. Describe Azure management and governance

# 1) Describe Cloud Concepts
## Intro to cloud computing.

## What is Cloud computing?
Cloud computing is the  delivery of computing services over the internet. These cloud computing include common IT infrastructure such as Virtual machines, storage, database hosting, and networking. And these also expand on offering services like IoT, ML and AI. 

Because cloud computing offers services over the internet, It doesn't have to constrained with infrastructure the same as traditional datacenter.
## What is Share responsibility model ?
To understand shared responsibility model first we need to understand how things are done at <ins>traditional datacenters.<ins>

* In traditional datacenters, The company is <u> Responsible</u> for maintaining the physical space, ensuring security, and maintaining or replacing the servers if anything happens. The IT department is responsible for maintaining all the infrastructure and software needed to keep the datacenter up and running. They’re also likely to be responsible for keeping all systems patched and on the correct version.

But, with shared responsibility model these <u>responsibilities </u> are shared between <u>cloud service provider and consumer.</u>

* Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider.
* At the same time, the consumer is responsible for the data and information stored in the cloud, The consumer is also responsible for access security, meaning you only give access to those who need it.

Then, for some things, the responsibility depends on the situation. If you’re using a cloud SQL database, the cloud provider would be responsible for maintaining the actual database. However, you’re still responsible for the data that gets ingested into the database. 

If you deployed a virtual machine and installed an SQL database on it, you’d be responsible for database patches and updates, as well as maintaining the data and information stored in the database

    The shared responsibility model is heavily tied into the cloud service types: infrastructure as a service (IaaS), platform as a service (PaaS), and software as a service (SaaS).
* IaaS places the most responsibility on the consumer, with the cloud provider being responsible for the basics of physical security, power, and connectivity. 
* On the other end of the spectrum, SaaS places most of the responsibility with the cloud provider.
* PaaS, being a middle ground between IaaS and SaaS, rests somewhere in the middle and evenly distributes responsibility between the cloud provider and the consumer.

### When using a cloud provider, you’ll always be responsible for: Fixed responsibilities

* The information and data stored in the cloud
* Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
* The accounts and identities of the people, services, and devices within your organization
### The cloud provider is always responsible for: Fixed responsibilities
* The physical datacenter
* The physical network
* The physical hosts
### Your service model will determine responsibility for things like:

* Operating systems
* Network controls
* Applications
* Identity and infrastructure
# Define Cloud Models ?
 The cloud models define the deployment type of cloud resources. The three main cloud models are: private, public, and hybrid.

### Private Cloud
A private cloud is, in some ways, the natural evolution from a corporate datacenter. It’s a cloud (delivering IT services over the internet) that’s used by a single entity. Private cloud provides much greater control for the company and its IT department. 

It may also be hosted in a dedicated datacenter offsite, potentially even by a third party that has dedicated that datacenter to your company.
### Public Cloud
A public cloud is built, controlled, and maintained by a third-party cloud provider. With a public cloud, anyone that wants to purchase cloud services can access and use resources. The general public availability is a key difference between public and private clouds.
### Hybrid Cloud
A hybrid cloud is a computing environment that uses both public and private clouds in an inter-connected environment.

Hybrid cloud can be used to provide an extra layer of security. For example, users can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure.
## Azure Arc
Azure Arc is a set of technologies that helps manage your cloud environment. Azure Arc can help manage your cloud environment, whether it's a public cloud solely on Azure, a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment running on multiple cloud providers at once.
## Azure VMware Solution
What if you’re already established with VMware in a private cloud environment but want to migrate to a public or hybrid cloud? Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.

# Describe the consumption-based model
When comparing IT infrastructure models, there are two types of expenses to consider. 

Capital expenditure (CapEx) and operational expenditure (OpEx).

Cloud computing falls under OpEx because cloud computing operates on a consumption-based model. With cloud computing, you don’t pay for the physical infrastructure, the electricity, the security, or anything else associated with maintaining a datacenter. Instead, you pay for the IT resources you use. If you don’t use any IT resources this month, you don’t pay for any IT resources.

This consumption-based model has many benefits, including:

* No upfront costs.
* No need to purchase and manage costly infrastructure that users might not use to its fullest potential.
* The ability to pay for more resources when they're needed.
* The ability to stop paying for resources that are no longer needed.
# Compare cloud pricing models
Cloud computing is the delivery of computing services over the internet by using a pay-as-you-go pricing model. You typically pay only for the cloud services you use, which helps you:

* Plan and manage your operating costs.
* Run your infrastructure more efficiently.
* Scale as your business needs change.

___
# Benefits of using cloud services
When building or deploying a cloud application, two of the biggest considerations are uptime (or availability) and the ability to handle demand (or scale).
## High availability
When you’re deploying an application, a service, or any IT resources, it’s important the resources are available when needed. High availability focuses on ensuring maximum availability, regardless of disruptions or events that may occur.

When you’re architecting your solution, you’ll need to account for service availability guarantees. Azure is a highly available cloud environment with uptime guarantees depending on the service. These guarantees are part of the service-level agreements (SLAs).
* Each service has different SLAs(service level agreements)
* In Azure some Services provide 99% availibility and some provide 99.99% availibility.
* 99% means 1.68 hr down time per week and 7 hr of down time per month.
* 99.99% means 10 min of down time per month and 43.2 min per month.

## Scalability
Scalability refers to the ability to adjust resources to meet demand. If you suddenly experience peak traffic and your systems are overwhelmed, the ability to scale means you can add more resources to better handle the increased demand.

    Scaling generally comes in two varieties: vertical and horizontal. Vertical scaling is focused on increasing or decreasing the capabilities of resources. Horizontal scaling is adding or subtracting the number of resources.


### Vertical scaling
With vertical scaling, if you were developing an app and you needed more processing power, you could vertically scale up to add more CPUs or RAM to the virtual machine. Conversely, if you realized you had over-specified the needs, you could vertically scale down by lowering the CPU or RAM specifications.

### Horizontal scaling
With horizontal scaling, if you suddenly experienced a steep jump in demand, your deployed resources could be scaled out (either automatically or manually). For example, you could add additional virtual machines or containers, scaling out. In the same manner, if there was a significant drop in demand, deployed resources could be scaled in (either automatically or manually), scaling in.
# Benefits of reliability and predictability in the cloud
Reliability and predictability are two crucial cloud benefits that help you develop solutions with confidence.

## Reliability
Reliability is the ability of a system to recover from failures and continue to function. It's also one of the pillars of the Microsoft Azure Well-Architected Framework.

This is achived by cloud de-centralization design, which naturally supports a reliability and resilient infrastructure.

With a decentralized design, the cloud enables you to have resources deployed in regions around the world. With this global scale, even if one region has a catastrophic event other regions are still up and running. You can design your applications to automatically take advantage of this increased reliability. In some cases, your cloud environment itself will automatically shift to a different region for you, with no action needed on your part. 

## Predictability
Predictability allowes you to move with confidence. This predictability is focused on <u>Performance predictability</u> and <u>Cost predictability.</u> These both are well influenced by MS Azure.

### Performance
This focuses on infrastructure or resources needed to delivery best experience for customers.
* Autoscaling, load balancing, and high availability are just some of the cloud concepts that support performance predictability.
* If you suddenly need more resources, autoscaling can deploy additional resources to meet the demand, and then scale back when the demand drops
* if the traffic is heavily focused on one area, load balancing will help redirect some of the overload to less stressed areas.
### Cost
This will help in forecasting the cost of the cloud spend.

    With the cloud, you can track your resource use in real time, monitor resources to ensure that you’re using them in the most efficient way, and apply data analytics to find patterns and trends that help better plan resource deployments.

* By operating in the cloud and using cloud analytics and information, you can predict future costs and adjust your resources as needed.
* You can even use tools like the Total Cost of Ownership (TCO) or Pricing Calculator to get an estimate of potential cloud spend.
## Benefits of security and governance in the cloud
### governance
Whether you’re deploying infrastructure as a service or software as a service, cloud features support governance and compliance.

Things like set templates help ensure that all your deployed resources meet corporate standards and government regulatory requirements. 

Plus, you can update all your deployed resources to new standards as standards change.

Cloud-based auditing helps flag any resource that’s out of compliance with your corporate standards and provides mitigation strategies. Depending on your operating model, software patches and updates may also automatically be applied, which helps with both governance and security.
### security
On the security side, you can find a cloud solution that matches your security needs. If you want maximum control of security, infrastructure as a service provides you with physical resources but lets you manage the operating systems and installed software, including patches and maintenance. If you want patches and maintenance taken care of automatically, platform as a service or software as a service deployments may be the best cloud strategies for you.

     And because the cloud is intended as an over-the-internet delivery of IT resources, cloud providers are typically well suited to handle things like distributed denial of service (DDoS) attacks, making your network more robust and secure.
# Benefits of manageability in the cloud
A major benefit of cloud computing is the manageability options. There are two types of manageability for cloud computing
### Management of the cloud
     Management of the cloud speaks to managing your cloud resources. In the cloud, you can:
* Automatically scale resource deployment based on need.
* Deploy resources based on a preconfigured template, removing the need for manual configuration.
* Monitor the health of resources and automatically replace failing resources.
* Receive automatic alerts based on configured metrics, so you’re aware of performance in real time.
### Management in the cloud
     Management in the cloud speaks to how you’re able to manage your cloud environment and resources. You can manage these:
* Through a web portal.
* Using a command line interface.
* Using APIs.
* Using PowerShell.

# Cloud service types:
### IaaS
 In an IaaS model, the cloud provider is responsible for maintaining the hardware, network connectivity (to the internet), and physical security. You’re responsible for everything else: operating system installation, configuration, and maintenance; network configuration; database and storage configuration; and so on. With IaaS, you’re essentially renting the hardware in a cloud datacenter, but what you do with that hardware is up to you.

 
Some common scenarios where IaaS might make sense include:

* Lift-and-shift migration: You’re setting up cloud resources similar to your on-prem datacenter, and then simply moving the things running on-prem to running on the IaaS infrastructure.
* Testing and development: You have established configurations for development and test environments that you need to rapidly replicate. You can start up or shut down the different environments rapidly with an IaaS structure, while maintaining complete control.
### PaaS
Platform as a service (PaaS) is a middle ground between renting space in a datacenter (infrastructure as a service) and paying for a complete and deployed solution (software as a service).

In a PaaS environment, the cloud provider maintains the physical infrastructure, physical security, and connection to the internet. They also maintain the operating systems, middleware, development tools, and business intelligence services that make up a cloud solution. 

Some common scenarios where PaaS might make sense include:

* Development framework: PaaS provides a framework that developers can build upon to develop or customize cloud-based applications. Similar to the way you create an Excel macro, PaaS lets developers create applications using built-in software components. Cloud features such as scalability, high-availability, and multi-tenant capability are included, reducing the amount of coding that developers must do.
* Analytics or business intelligence: Tools provided as a service with PaaS allow organizations to analyze and mine their data, finding insights and patterns and predicting outcomes to improve forecasting, product design decisions, investment returns, and other business decisions.
### SaaS
Software as a service (SaaS) is the most complete cloud service model from a product perspective. With SaaS, you’re essentially renting or using a fully developed application. Email, financial software, messaging applications, and connectivity software are all common examples of a SaaS implementation.

Some common scenarios for SaaS are:

* Email and messaging.
* Business productivity applications.
* Finance and expense tracking.




