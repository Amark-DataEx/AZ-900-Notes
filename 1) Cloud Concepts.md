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