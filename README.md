# INTRO-TO-CLOUD-COMPUTING-UDACITY

# LESSON 1

## 1. Meet your instructor 

### Ami Maloof
My name is Ami Mahloof and I am a senior cloud architect. My experience with cloud computing goes back to the early days of AWS, around 2008, when AWS used to have EC2 
and S3 services with very basic functionality. In my career, I've managed production workloads with millions of users, on multiple cloud providers: AWS, GCP, Azure, 
Alibaba Cloud, and Rackspace.

I've designed and built architectures for automatic scaling, high availability, machine learning, monitoring, and more. I've automated most of the cloud operations
programmatically and even extended some cloud services by myself.

I have over 10 years of experience with AWS. In this course, I will be teaching you to work with and integrate basic cloud services.

## 2. Course Outline

In this course, we will cover:

* Overview of cloud computing, benefits, major providers, and cost management
* Cloud computing fundamentals, characteristics, and virtualization
* AWS console access, and AWS services
* Compute services
* Databases, and serverless architecture

![](https://video.udacity-data.com/topher/2020/June/5ed9e8ed_course-outline/course-outline.png)

### Learning Objectives
At the end of this course you will be able to:

* Navigate and interact with the AWS services in the console
* Create cloud identities and policies to access the cloud services
* Store files in an S3 bucket
* Launch a Linux Virtual Machine (AWS EC2 instance)
* Automate EC2 instance provisioning via an init script that will retrieve data from an S3 bucket
* Create a serverless app for storing users' names and greeting them when they return, using serverless architecture (API Gateway, Lambda, and a Redis database)

## 3. Lesson Outline

This lesson covers the benefits of cloud computing, the major cloud providers currently, deployment model, and estimating costs for running services in the cloud.

![](https://video.udacity-data.com/topher/2020/June/5ed9ea8f_iccfc-l1-outline/iccfc-l1-outline.png)

### Learning Objectives
By the end of this lesson, you will be able to:

* Explain the benefits of cloud computing
* Differentiate between cloud service providers
* Choose when to use a public versus private deployment model
* Estimate cloud costs based on the AWS calculator

## 4. Cloud Computing
Cloud computing is a collection of online managed services (especially data storage and computing power) owned, run, and maintained by a cloud provider, without direct active management from users. Pay for what you use.

### Users
Organizations of any type, size, or industry use cloud computing. For example:

* Mobile apps companies
* Websites
* Large organizations with extended IT services
* Video streaming platforms Netflix, Hulu, youtube…
* Online video games
* Developers that need to work together in a shared environment

![](https://video.udacity-data.com/topher/2020/June/5ed9ec1f_cloud-users/cloud-users.png)

## 5. Benefits of Cloud Computing

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/1.jpg?token=ADDIJ7KWRGZXAFYN7U42KJDANB5Q4)

### Agility
The cloud is agile. Infrastructure resources can spin up when necessary. Among these resources are compute, storage, databases, Internet of things (IoT), machine learning, analytics, and more.

### Elasticity
The cloud has the ability to handle peak levels of business activity automatically and on-demand, by scaling resources up or down to shrink or grow capacity when the business needs change.

### Economy
Because cloud computing removes the traditional costs of owning and maintaining hardware, and payment is only for usage, the cost savings are very large. On top of that cloud computing providers offer steep discounts for some resources, such as compute, if the workflow on them can be interrupted. This even further increases the cost-savings of running in the cloud.

### Availability
Cloud computing providers offer their services in many locations within a geographical region, and in many locations around the globe. This extends the availability and durability of cloud services.

### QUIZ QUESTION
What are 3 benefits of cloud computing?

* Elasticty
* Economy
* Scalability

## 6. Cloud History

In the early days of the Internet, before cloud computing, hosting providers allocated shared servers where one could run and install a monolithic app. This approach
encountered challenges to scalability and resiliency, as well as security risks.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/2.jpg?token=ADDIJ7JF3HN6JR32CXKKTYDANB6E6)

Cloud computing became popular in 2006, when Amazon.com released its "Elastic Cloud Compute" service, known as EC2 ('E' for elastic and 2 'C's for Cloud Compute). Cloud computing addresses many of the challenges faced by early application platforms.

The word "cloud" has long been a metaphor for the Internet, and the cloud symbol was used in network telephony schematics all the way back to the 1970s.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/3.jpg?token=ADDIJ7OFTLEIPQMVPSALQ7DANB6GK)

Since 2006, other cloud providers have surfaced. Additionally, many more services have been incorporated into the cloud, to minimize different self-managed services 

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/4.jpg?token=ADDIJ7KBXLO5VMZQ4G256LDANB6IK)

necessary to run different types of web applications.

### QUIZ QUESTION
In what year did cloud computing become popular?

* 2006

## 7. Cloud Stakeholders
The cloud matters to many few types of people in an organization:

* A CFO would be interested in budgets and costs for running in the cloud
* A developer would be interested in building an app or a platform in the cloud
* The IT department would be interested in centralizing, extending, and backing up on-premise data
* DevOps would be interested in improving uptime, responsiveness, and efficiency
* Marketing and Product Management would be interested in the analytics capabilities of the cloud

![](https://video.udacity-data.com/topher/2020/June/5ed9f304_cloud-stakeholders/cloud-stakeholders.png)

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/5.jpg?token=ADDIJ7O4XZ3LNIL4GTIHRKDANB6XE)

## 8. Types of Cloud Computing

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/6.jpg?token=ADDIJ7L36HYNO6CMC5HJXZDANB7BO)

### Infrastructure as a service
Infrastructure as a service (IaaS), also known as cloud infrastructure services, are highly scalable and automated computing resources.

IaaS is fully self-service for accessing and monitoring computers, networking, storage, and other services.

This model allows businesses to purchase resources on-demand and as-needed, instead of having to buy the hardware outright.

### IaaS Characteristics
* Resources are available as a service
* Cost varies depending on consumption
* Services are highly scalable
* Multiple users share a single piece of hardware
* Organization retain control of the infrastructure
* Dynamic and flexible

### Platform as a service (PaaS)
Platform as a service (PaaS), also known as cloud platform services, allows developers to build upon a framework to create custom applications. By obstructing or hiding servers, storage, and networking, PaaS providers help developers focus on managing their applications, rather managing the base infrastructure. Heroku is an example of a PaaS provider.

### PaaS Characteristics
* Builds on virtualization technology, so resources can easily be scaled up or down
* Provides a variety of services to assist with the development, testing, and deployment of apps
* Accessible to numerous users via the same development application
* Integrates web services and databases

### Software as a service (SaaS)
The most common option for cloud use, allowing 3rd-party vendors to deliver applications that run in the browser, without any installation. For example, G Suite is a SaaS solution for office apps in your browser.

### SaaS characteristics:
* Managed from a central location
* Hosted on a remote server
* Accessible in a browser (sometimes even when the user is offline)
* Users are not responsible for hardware or software updates

## 9. Quiz: Types of Cloud Computing

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/7.jpg?token=ADDIJ7LEKUACRH4YS4TFFPTANCAMO)

## 10. Deployment Models

### Cloud Deployment Models

### Public Deployment
The Public Deployment model is the most common deployment model. Services face the Internet and share hardware, network, and storage across many organizations and tenants.

### Advantages
* Cost-effective
* Pay-as-you-go - only pay for resources you use
* Maintenance-free - the cloud provider is responsible

### Private Deployment
The Private Deployment model limits each deployment to a single organization. This model provides better control of network security. Resources are not shared between organizations and tenants, which reduces risk.

The private cloud can be an on-premise or it can be hosted by a cloud provider. Even if the deployment is hosted by a cloud provider, all of the hardware and software is dedicated to one organization.

The Private Deployment model is often used by governments, financial institutions, or organizations that must comply with strict regulatory protocols

### Advantages
* Supports highly customized networks
* Facilitates tighter security and privacy
* Provides greater control over infrastructure

### Hybrid Deployment
The Hybrid Deployment model is a mix of the Public and Private Deployment models, combining the benefits of both.

This model offers the flexibility of running on private infrastructure, but the model can switch to the public cloud when permissible, to realize the benefits such as cost-savings.

In Hybrid Deployment data can flow from the private cloud to the public cloud and vice versa.

The downside of a hybrid deployment model is the cost of configuring and maintaining services across both types of clouds.

![](https://video.udacity-data.com/topher/2020/June/5edbf872_hybrid-cloud/hybrid-cloud.png)

## 11. Quiz: Deployment Models

### QUESTION 1 OF 2
Which of the following is the most cost-effective deployment model?

* Public

### QUESTION 2 OF 2
Which network configuration would be typical of a private deployment model?

* 1 IP address: 10.0.0.20

## 12. Major Providers

### Major Cloud Providers
* Amazon Web Services (AWS)
* Google Cloud Platform (GCP)
* Microsoft Azure

At a high level, these providers are similar. However, there are many factors that distinguish them from each other, including:

* Geographic Availability
* Market Share and Growth Rate
* Services
* Pricing Model

### Geographic Availability
Cloud computing locations are worldwide. These locations called "regions" and "availability zones."

Each region is a separate geographic area. Within each region, there are multiple isolated locations known as availability zones.

This geographic spread provides the ability to place resources, such as compute and storage, closer to end-users for faster access and better performance.

The number of regions and the availability zones within them differs between cloud providers.

* AWS has 18 regions and between 2-6 availability zones per region
* GCP has 23 regions with at least 3 availability zones per region
* Azure has 58 regions worldwide and is available in 140 countries all around the world

The geographic locations between each cloud providers are different. One example is that currently the only cloud provider that can work in mainland China is AWS GCP offers a region in Hong Kong, but those resources are not always accessible from mainland China.

And there are other key factors such as submarine networking between geographic locations.
 
![](https://video.udacity-data.com/topher/2020/June/5edc02ac_major-cloud-providers-geography/major-cloud-providers-geography.png)

### Market Share And Growth Rate
* AWS has been around since 2006 and is currently the leading cloud provider, with 33% market share
* Microsoft Azure holds about 17% worldwide market share
* Google has about 6% percent of the market worldwide

While this doesn't add up to 100%, remember that there are many other cloud providers that, in aggregate, make up the entire cloud computing market.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/8.jpg?token=ADDIJ7PEOWV2PDVL7F3GH5LANCDGK)

### Services
* AWS offers 200+ services, ranging from computing, storage, and databases through machine learning and artificial intelligence (AI) to Internet of Things (IoT), analytics, and more
* GCP offers about 50+ services, similar to AWS
* Azure offers about 30+ services, with a focus on integration with other Microsoft tools

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/9.jpg?token=ADDIJ7OTA33GZK345ODQ6E3ANCDMI)

### Pricing
The pricing models of the major cloud provides are similar:

* On-demand, pay-as-you-go
* Discounts for committed usage
* Usage-based serverless resources

On-demand pricing for the same compute (CPU-RAM-Disk) resources varies between cloud providers and is calculated on an hourly rate.

Discounts also vary between cloud providers. For example, AWS offers reserved instances that you can pre-purchase annually, whereas GCP offers "sustained use discount" whereby pricing goes down the more you use an instance.

Serverless computing (Lambda on AWS, Functions on Azure, and Cloud Functions on GCP) are billed for the compute power you use, based on 100-millisecond increments.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING-UDACITY/master/images/10.jpg?token=ADDIJ7I3XGYEBYDHZE7RHSDANCDSI)


