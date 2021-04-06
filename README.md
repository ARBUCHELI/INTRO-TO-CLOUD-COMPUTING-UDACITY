# INTRO-TO-CLOUD-COMPUTING-UDACITY

# LESSON 1 OVERVIEW

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

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/1.jpg)

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

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/2.jpg)

Cloud computing became popular in 2006, when Amazon.com released its "Elastic Cloud Compute" service, known as EC2 ('E' for elastic and 2 'C's for Cloud Compute). Cloud computing addresses many of the challenges faced by early application platforms.

The word "cloud" has long been a metaphor for the Internet, and the cloud symbol was used in network telephony schematics all the way back to the 1970s.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/3.jpg)

Since 2006, other cloud providers have surfaced. Additionally, many more services have been incorporated into the cloud, to minimize different self-managed services 

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/4.jpg)

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

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/5.jpg)

## 8. Types of Cloud Computing

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/6.jpg)

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

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/7.jpg)

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

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/8.jpg)

### Services
* AWS offers 200+ services, ranging from computing, storage, and databases through machine learning and artificial intelligence (AI) to Internet of Things (IoT), analytics, and more
* GCP offers about 50+ services, similar to AWS
* Azure offers about 30+ services, with a focus on integration with other Microsoft tools

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/9.jpg)

### Pricing
The pricing models of the major cloud provides are similar:

* On-demand, pay-as-you-go
* Discounts for committed usage
* Usage-based serverless resources

On-demand pricing for the same compute (CPU-RAM-Disk) resources varies between cloud providers and is calculated on an hourly rate.

Discounts also vary between cloud providers. For example, AWS offers reserved instances that you can pre-purchase annually, whereas GCP offers "sustained use discount" whereby pricing goes down the more you use an instance.

Serverless computing (Lambda on AWS, Functions on Azure, and Cloud Functions on GCP) are billed for the compute power you use, based on 100-millisecond increments.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/10.jpg)

## 13. Quiz: Major Cloud Providers

### QUIZ QUESTION
What are the key factors distinguishing between the major cloud providers?

* Geographic Availability in Regions and Zones
* Pricing Models
* Services
* Market Shares and Growth Rate

## 14. Costs

### Costs In The Cloud
Cost savings is one of the reasons why companies are moving into the Cloud, but these costs can get out of hand easily.

Cloud providers supply up-to-date pricing information for all of their services and components.

Let's explore one way to estimate the costs for the infrastructure we need on AWS using the [AWS Pricing Calculator](https://calculator.aws/#/).

## 15. Quiz: Costs Overview

### Quiz: Costs
### QUESTION 1 OF 2
Which tool estimates a service's end-to-end costs?
* AWS Pricing Calculator

### QUESTION 2 OF 2
If the cost of a t2.medium is $0.04 per hour, approximately how much would it cost to run an instance for the whole month of January?
* $30

##  16. Exercise: AWS Pricing Calculator

In this exercise, you will use the [AWS Pricing Calculator](https://calculator.aws/#/) to estimate the costs for a hypothetical upload and resize service hosted on AWS.

The service architecture is:

* Compute and storage run in the ```us-west-2 Oregon``` region
* One (1) EC2 ```t2.medium on-demand``` instance with a root volume of ```250GB```
* One (1) S3 bucket with a ```Standard``` storage class, which will store the resized images
* The size of the uploaded images will not exceed: ```200GB``` per month
* The resized image requires ```1MB``` of S3 storage
* The server disk space is cleaned up monthly

Factors you should take into account for the cost estimate:

* There is no charge for <strong>inbound data transfer</strong> across all services in all regions
* A write operation to S3 is known as a PUT request

### Expected Result
If your estimate is correct, your total monthly cost should be approximately <strong>64.47 USD.</strong>

## 17. Solution: AWS Pricing Calculator

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/11.jpg)](https://www.youtube.com/watch?v=cMni87XTRbo&feature=emb_logo)

### Solution
The following is a solution for the AWS Pricing Calculator exercise.

We will first disaggregate the cloud services. Then we will configure the attributes of each service in the [AWS pricing calculator](https://calculator.aws/#/).

### Breakdown
The upload service is built on top of 2 cloud services:

* EC2 for compute
* S3 for cloud storage

Region for service: ```us-west-2 (Oregon)``` region

### EC2 Information We Know
* The EC2 instance payment model is ```on-demand```
* There is one EC2 instance of ```t2.medium``` type
* The size for root storage on the instance is ```250GB```

### S3 Information We Know
* The default storage class for S3 is ```standard``` which is what the service will use
* We will be storing ```200GB``` of images per month
* Each image stored on S3 will be 1MB
* A write operation in S3 is known as ```Put request```, so if we convert the 200GB to MB we should get 200,000MB (multiply the digital storage value by 1000)

### Walkthrough
### EC2 Cost Estimation
Open up the [AWS Pricing Calcuator](https://calculator.aws/#/)

Click on the <strong>Create estimate</strong> button

Type <strong>ec2</strong> in the <strong>AWS services</strong> filter box, then click on the <strong>configure</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e84f9fb_ec2-configure/ec2-configure.png)

Change the ```Region``` dropdown to ```US West (Oregon)``` and leave the default option to create a Quick estimate.

Choose the option of ```Search instances by name``` and Enter ```t2.medium``` for the instance type

![](https://video.udacity-data.com/topher/2020/April/5e84f9f9_screen-shot-2020-04-01-at-12.17.23/screen-shot-2020-04-01-at-12.17.23.png)

Scroll down the ```Pricing strategy``` box and choose ```On-Demand instances```

![](https://video.udacity-data.com/topher/2020/April/5e850644_aws-calculator-ec2-pricing-strategy/aws-calculator-ec2-pricing-strategy.png)

Scroll down the ```Pricing strategy``` box and choose ```On-Demand instances```

Now let's configure the root size of the ```Elastic Block Storage (EBS)``` which is the disk connected to the instance.

The default is ```General Purpose SSD (gp2)``` which is what we want so we just need to change the ```Storage amount to 250GB```

![](https://video.udacity-data.com/topher/2020/April/5e850698_aws-calculator-ec2-ebs/aws-calculator-ec2-ebs.png)

At this point we can already tell that the EC2 would cost us $58.87 USD monthly, That's all we need for the EC2 section, so let's click the ```Add to my estimate``` button

![](https://video.udacity-data.com/topher/2020/April/5e85071c_aws-calculator-ec2-summry/aws-calculator-ec2-summry.png)

### Configure The S3 For The Service
Now that we have the estimate built for our compute section let's add to it the S3 storage service.

Click the ```Add service``` button to add a new service, then type ```s3``` in the AWS services filter box, notice how other services that use S3 also coming up in the search as the filter look up the description too.

scroll down and look for the actual service, S3 is called ```Simple Storage Service``` these 3 Initials are all starting with the letter S which is 3S => S3

![](https://video.udacity-data.com/topher/2020/April/5e8507cb_aws-calculator-s3-intro/aws-calculator-s3-intro.png)

Click on the ```Configure``` button on the ```Amazon Simple Storage Service``` button to configure the S3 service.

Make sure the region is set to ```US West (Oregon)```

un-toggle all of the Storage classes but the ```S3 Standard``` as well as the ```Data Transfer``` as we are not going to pull data from S3 and all Incoming traffic is free.

![](https://video.udacity-data.com/topher/2020/April/5e8507ca_aws-calculator-s3-storage-class/aws-calculator-s3-storage-class.png)

We know that the service will be uploading 200GB per month of images so let's configure the storage amount to 200GB per month

and under the ```PUT, COPY, POST, LIST requests to S3 standard``` type 200,000

scroll down to the bottom of the page and click the ```Add to my estimate``` button

![](https://video.udacity-data.com/topher/2020/April/5e8507c9_aws-calculator-s3-storage/aws-calculator-s3-storage.png)

Your S3 cost should come up to somewhere around <strong>$5.60 USD</strong>

![](https://video.udacity-data.com/topher/2020/April/5e8507c8_aws-calculator-s3-summary/aws-calculator-s3-summary.png)

Your Estimate should come up to somewhere around <strong>$64.47 USD</strong>

Please keep in mind that pricing always changes and is dynamic.

![](https://video.udacity-data.com/topher/2020/April/5e85092d_aws-calculator-estimate/aws-calculator-estimate.png)

## 18. Edge Cases

### When Not to Use The Cloud
There are situation in which the costs of running in the cloud surpass the costs of running and maintaining a set of servers.

One example is GPU machine learning. While the cloud can provide cost optimization for GPU instances via spot instance discounts, often the cost of running a set of cloud GPU instances would be much higher than the cost to buy and maintain your own set of GPU servers.

Other examples include the Private deployment model, which might be on-premise for security or regulatory reasons.

Even though the cloud has many managed services, cloud applications still require an experienced engineer with security, networking, and cloud skills to maintain the application. If an organization lacks such a person, the cloud might not be a good option.

### QUIZ QUESTION
When should you avoid the cloud?

* When regulations or company policy prohibit you from running in a multi-tenant environment
* When you lack the expertise to utilize cloud services

## 19. Intuition

### Intuition
Even though this course is aimed at beginners, we will nonetheless study security, networking, and best practices. In my experience working alongside many beginners, their focus was, "First let's just get it working," without thinking about security or designing a network for their needs. The results were problematic since the work had to be redone.

In this course, you'll learn to work with cloud resources the "right" way.

### 20. Lesson Recap

In this lesson we covered:

* What is cloud computing and who uses it
* Benefits of cloud computing
* Types of cloud computing
* Deployment models
* Major cloud providers
* Estimating cloud costs

![](https://video.udacity-data.com/topher/2020/June/5ed9e8ed_course-outline/course-outline.png)

### Course Outline
In the rest of this course, we will study:

* Cloud Fundamentals
* AWS Console and AWS Services
* Compute Services
* Serverless Architechture

### Further Reading
### Documentation
[AWS Getting Started](https://aws.amazon.com/es/getting-started/)

### Books
[Introduction to Amazon Web Services Beginners Guide Book](https://www.amazon.com/Introduction-Amazon-Services-Beginners-Guide/dp/1539751953)

### Research Papers
[AWS Well-Architected White Papers](https://aws.amazon.com/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc)

### Blogs
[AWS Blog](https://aws.amazon.com/blogs/aws/)

## 21. Glossary

<strong>Agility:</strong> The ability of a company to build and operate infrastructure quickly and easily.

<strong>Elasticity:</strong> The ability to shrink or grow the capacity of cloud resources.

<strong>Private Deployment:</strong> A model whereby resources are not shared between organizations and tenants (can be on-premise or in the cloud).

<strong>Public Deployment:</strong> A model whereby services face the internet and resources such as hardware, storage, and network are shared between organizations to reduce costs.

<strong>Hybrid Deployment:</strong> A mix of public and private deployment models.

## 22. Build your career

### Build Your Career: Udacity Cloud Computing Nanodegree Programs
Thanks for enrolling in our Introduction to Cloud Computing course and congratulations in taking the first step toward an exciting career in cloud computing. The global public cloud computing market is expected to reach over $600 billion by 2023 and cloud professionals are in high demand. Continue to build your career in one of Udacity’s Cloud Computing Nanodegree Programs. Watch the videos below to learn more and click on the name of each Nanodegree to start today!

[Cloud Developer Nanodegree Program](https://www.udacity.com/course/cloud-developer-nanodegree--nd9990)

Learn the fundamentals of cloud development and deployment with AWS. Then, build different apps leveraging microservices, Kubernetes clusters, and serverless application technology.

[Cloud DevOps Engineer Nanodegree Program](https://www.udacity.com/course/cloud-dev-ops-nanodegree--nd9991)

Develop the skills you need to join the rapidly growing cloud devops field. With the help of expert instructors and mentors, you’ll learn to deploy apps and infrastructure as code on AWS, build CI/CD pipelines, and operationalize microservices at scale using Kubernetes.

[AWS Cloud Architect Nanodegree Program](https://www.udacity.com/course/aws-cloud-architect-nanodegree--nd063)

Play a critical role in an organization’s cloud computing strategy as an AWS Cloud Architect. Learn to plan, design, and implement secure cloud infrastructure in AWS at scale. Begin by designing and building high availability infrastructure, and then move on to building scalable, secure, and cost-optimized architecture. Finally, explore and execute best practices and strategies around securing access to cloud services and infrastructure.

_________________________________________________________________________________________________________________________________________________________________________________

# LESSON 2 FUNDAMENTALS

## 1. Fundamentals

### Cloud Computing Fundamentals
The fundamentals of cloud computing include both virtualization and characteristics specific to the cloud.

* Managed services
* On-demand services
* Scalability
* Elasticity
* Security

Virtualization allows cloud providers to share compute, storage, and networking across cloud users. This is the heart of cloud computing.

![](https://video.udacity-data.com/topher/2020/June/5ed9e8ed_course-outline/course-outline.png)

### Course Outline
In this lesson we will focus on:

* Cloud computing characteristics
* Virtualization

In future lessons we will cover:

* AWS console, and AWS services
* Compute services and Virtual Private Cloud
* Databases, and serverless architecture

## 2. Lesson Outline

* Multi tenant hosts
* Managed and on-demand services
* Networking
* Elasticity and Scalability
* Security
* Virtualization and virtual machines

### Lesson
This lesson covers virtualization and the characteristics of cloud computing.

### Learning Objectives
By the end of this lesson, you will be able to:

* Pick the right cloud service for your needs
* Bring up a virtual machine on your own computer

![](https://video.udacity-data.com/topher/2020/June/5edc0f2d_iccfc-lesson-2-outline/iccfc-lesson-2-outline.png)

## 3. Cloud Characteristics

* <strong>Managed services</strong> are operated and maintained by the cloud provider on your behalf

* <strong>On-Demand Services</strong> are available to use and release instantly; only pay for what you use

* <strong>Virtual Private Clouds</strong> allows network customization with grater security and isolation

* <strong>Scalability & Elasticity</strong> refer to the ability of your cloud resources to grow or shrink on-demand

* <strong>Security</strong> includes both network security and access management

![](https://video.udacity-data.com/topher/2020/June/5edc1125_cloud-characteristics/cloud-characteristics.png)

## 4. Quiz: Cloud Characteristics

### QUESTION 1 OF 2
A user is responsible for installing, maintaining and running a managed service.

* False

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/12.jpg)

## 5. Virtualization

* Many virtual machines can run on a single host os
* You can run a VM either on your own local computer or in the cloud
* Virtual machines running on the same host are isolated from each other
* Each VM requires an entire operating system (Linux, Windows, etc.)

![](https://video.udacity-data.com/topher/2020/June/5edc133a_virtual-machines/virtual-machines.png)

A host machine has memory, CPU, storage, and networking. The host runs a program called a "hypervisor", which manages multiple "virtual machines", each of which can run its own applications.

## 6. Quiz: Virtualization

### QUESTION 1 OF 3
Can you run both Windows and Linux virtual machines on macOS?
* Yes

### QUESTION 2 OF 3
What is the software core component that makes virtualization happen?
* Hypervisor

### QUESTION 3 OF 3
What is a VM?
* A virtual machine, which runs its own operating system and shares some of the physical host's resources

## 7. Exercise: Virtualization

You are about to use a hypervisor called VirtualBox to bring up a Linux Ubuntu virtual machine on your own computer!

Cloud computing relies heavily on virtualization. Launching your own virtual machine is great preparation for working with cloud resources.

VirtualBox is open-source software that you can install on your own computer. This hypervisor allows you to run a "guest" operating system on top of your own "host" operating system.

This flexibility allows, for example, a Windows VM on a macOS or Linux host.

VirtualBox also allows you to allocate part of the host's resources (CPU, memory, disk) to the guest OS.

Cloud Computing works similarly. For example, one physical host (which cloud customers typically cannot access) can run many Instances, akin to guests.

### VirtualBox Installation
Head over to [VirtualBox's Download page](https://www.virtualbox.org/wiki/Downloads) and download the right copy for your system under the <strong>VirtualBox platform packages</strong> section.

Open up installation executable and click through the setup dialogs.

Once VirtualBox is installed, launch it and you will see the <strong>Welcome to VirtualBox</strong> window.

### Exercise Requirements
* VirtualBox version 6 (or higher)
* Download the [Ubuntu 19.04 (64-bit) VirtualBox disk image](https://www.osboxes.org/ubuntu/)
* Extract the image using:
>> * Linux: [p7zip](http://p7zip.sourceforge.net/)
>> * macOS: [Keka](https://www.keka.io/en/)
>> * Windows: [7zip](https://www.7-zip.org/download.html)

![](https://video.udacity-data.com/topher/2020/April/5e86b74a_vbox-welcome/vbox-welcome.png)

### Exercise

* Allocate 512MB of memory to the VM
* For the Hard Disk, select the option ```Use existing virtual hard drive file``` and point to the downloaded image which should be in a ```VDI``` format
* From the VM settings -> Display tab, drag the ```Scale Factor``` slider all the way to the right (300%)
* Start the VM and use the <strong>Password:</strong> ```5osboxes.org``` to login
* Stop the VM and resize the amount of memory to ```1024MB``` via ```Settings``` -> ```System```
* Resize the number of allocated CPU's to ```2```
* Start the VM again, login and check the Memory and CPU count matching via the Apps icon (grid on the bottom of the dock) and ```Details```

## 8. Solution: Virtualization

### Solution: Creating A New Virtual Machine From A Virtual Disk Image
Once VirtualBox is installed, and the Ubuntu 19.04 (64-bit) <strong>virtual disk image VDI</strong> is extracted, we will create a new Virtual Machine from it.

Open up VirtualBox app, you should see the empty dialog box: <strong>Welcome to VirtualBox</strong>

Click the <strong>New</strong> button and set the following:

* <strong>Name:</strong> Ubuntu
* <strong>Type:</strong> Linux
* <strong>Version:</strong> Ubuntu (64-bit)

Then click Continue.

![](https://video.udacity-data.com/topher/2020/April/5e86c1ff_vbox-1/vbox-1.png)

Click Continue and set the <strong>Memory Size</strong> to 512MB.

![](https://video.udacity-data.com/topher/2020/April/5e86c1ff_vbox-2/vbox-2.png)

On the Hard Disk setup, choose the <strong>Use an existing virtual hard disk file option</strong>.

![](https://video.udacity-data.com/topher/2020/April/5e86c632_screen-shot-2020-04-02-at-22.14.15/screen-shot-2020-04-02-at-22.14.15.png)

Then, click the folder icon to the right to browse to the file location.

Note that you can choose the option <strong>VDI</strong> from the dropdown box.

The file should be in the Downloads folder and should be inside of a folder called <strong>64bit</strong>

Select the <strong>Ubuntu 19.04 (64bit).vdi</strong> file followed by the <strong>Open</strong> button.

![](https://video.udacity-data.com/topher/2020/April/5e86c1fe_vbox-3/vbox-3.png)

Before you start the VM, we need to set the screen size to a normal working size. To do that, click the VM settings, Display tab and drag the <strong>Scale Factor</strong> slider all the way to the right and set it at 300%.

![](https://video.udacity-data.com/topher/2020/April/5e86c1fa_vbox-8/vbox-8.png)

Now, start the VM. Log in as "osboxes.org" use the password "osboxes.org" to login.

Skip <strong>Connect your online account</strong>

Ignore the message about upgrades and click through the welcome screen.

![](https://video.udacity-data.com/topher/2020/April/5e86c1f9_vbox-9/vbox-9.png)

![](https://video.udacity-data.com/topher/2020/April/5e86c1f5_vbox-11/vbox-11.png)

### Resizing the VM
Stop the VM.

Go back into the settings and click on the System tab.

The default tab on this settings is <strong>Motherboard</strong>

Set the <strong>Base Memory</strong> to 1024MB.

![](https://video.udacity-data.com/topher/2020/April/5e86c1fd_vbox-4/vbox-4.png)

Click on the <strong>Processor</strong> tab on the top and set the CPU count to 2.

![](https://video.udacity-data.com/topher/2020/April/5e86c1fb_vbox-5/vbox-5.png)

Once you click OK, you can see the changes in the info screen.

![](https://video.udacity-data.com/topher/2020/April/5e86c1fb_vbox-6/vbox-6.png)

Start the VM again, click on the APPs icons (Grid Icon) on the dock to the left and choose the System Settings icon.

On the bottom of it, you should see the <strong>Details</strong> section. Click on it and verify that the CPU and memory are matching the new settings.

![](https://video.udacity-data.com/topher/2020/April/5e86c1f3_vbox-12/vbox-12.png)

### Conclusion
Congratulations! You have launched a virtual machine on your local computer!

This is a major step toward understanding how cloud computing works.

You might wonder how many VMs you could launch on your local machine. Could your local machine become a cloud provider, all by itself?

The number of VMs that can be launched on a physical host depends on the shared resources allocations. Your local machine probably has enough resources to comfortably support several VMs, but nothing on the scale of a cloud provider.

The concept of virtualization maps directly to cloud computing, though. Multiple tenants can share the resources of a physical host, with a separation between the VM guests.

Cloud computing offers dedicated hosts, too. This means that the entire physical host is dedicated to a single customer.

One use case for that would be launching a few virtual machines on the same physical host, for better placement and performance. A risk, however, is that this host becomes of a single point of failure for all of these instances.

## 9. Edge Cases

### When Not To Use A VM
Remember that a VM acquires resources from the host computer. An idling or underutilized VM, which does not need its full computing power, drains resources the host could use for other tasks or share with other VMS.

In the case of underutilization, a [container](https://www.docker.com/resources/what-container) or [serverless](https://blog.hubspot.com/website/serverless-functions) function might be a better choice.

On the other end of the spectrum, a VM might need more resources than the host can provide. In this case, a [dedicated](https://aws.amazon.com/es/ec2/pricing/dedicated-instances/) server might be a better choice.

QUIZ QUESTION
What characteristics matter when deciding whether to use a VM?

* Idling processes
* Underutilizied VM
* Overutlizised VM

## 10. Lesson Recap

In this lesson you:

* Learned about virtualization and cloud computing characteristics
* Launched a virtual machine on your own computer!

In the next lesson, you will:

* Sign up for Amazon Web Services
* Navigate and interact with the AWS console
* Create an IAM user
* Configure an IAM policy
* Launch an S3 bucket to store files in the cloud

![](https://video.udacity-data.com/topher/2020/June/5edc1e7b_course-outline/course-outline.png)

### Further Reading
### Documentation
* [Virtualbox documentation](https://www.virtualbox.org/wiki/Documentation)
* [Understanding Virtualization by RedHat](https://www.redhat.com/en/topics/virtualization)
* [Virtualization - a complete guide by I.B.M](https://www.ibm.com/cloud/learn/virtualization-a-complete-guide)

### Books
* [Virtualization Essentials](https://www.amazon.com/Virtualization-Essentials-Matthew-Portnoy/dp/1118176715)

### Research Papers
* [Research on the Virtualization Technology in Cloud Computing Environment](https://www.researchgate.net/publication/297603485_Research_on_the_Virtualization_Technology_in_Cloud_Computing_Environment)

### Blogs
* [An introduction to virtualization](https://medium.com/@rohithaelsa/an-introducton-to-virtualization-b67a58bee4e8)
* [Virtualization basics](https://medium.com/@jain.sm/virtualization-basics-dad2f20067e6)

## 11. Glossary

<strong>Guest:</strong> The operating system that runs inside a virtual machine.

<strong>Host:</strong> The physical computer running the guest VM.

<strong>Hypervisor:</strong> Software that manages virtual machines and facilitates hardware emulation for the guest VMs.

<strong>Managed Services:</strong> A set of services that the cloud provider runs and operates on your behalf.

<strong>Virtual Machine:</strong> An isolated environment that acts and behaves like a real computer, and runs on a host machine, sharing its resources.

<strong>Virtualization:</strong> A technology that allows for the creation of software-based virtual machines that can run multiple operating systems from a single physical machine.

_________________________________________________________________________________________________________________________________________________________________________________

# LESSON 3 AWS CONSOLE & ACCESS

## 1. AWS Console and Access

### AWS Console and Access
The AWS console is the user interface that allows access and configuration of services.

One of the services for controlling that access is called IAM - Identity And Access Management. With IAM you can create identities and policies to configure access to resources.

In this lesson, you will create an S3 bucket as well as IAM users to access and upload content to that bucket.

More specifically, you will create IAM policies to allow access to that S3 bucket and specify the actions a user can perform.

![](https://video.udacity-data.com/topher/2020/June/5edc6e07_course-outline/course-outline.png)

## 2. Lesson Outline

## Course Outline
So far in this course, we have covered:

* Overview
* Fundamentals

In this lesson, we will focus on:

* AWS console and AWS services
* Identity and Access Management (IAM)
* Creating IAM User and Policies
* Creating and using S3 bucket

In future lessons we will cover:

* Compute services
* Databases and serverless architecture

![](https://video.udacity-data.com/topher/2020/June/5edc6f1b_course-outline/course-outline.png)

### Lesson Outline
This lesson covers signing up for AWS, navigating and interacting with AWS services via the console, and creating

* IAM users
* IAM policies
* S3 buckets

### Learning Objectives
By the end of this lesson, you will be able to:

* Sign up for AWS services
* Secure your AWS root account using multi-factor authentication
* Navigate AWS services via the console
* Create an S3 bucket
* Create an IAM user
* Configure an IAM inline policy to permit reading and writing to an S3 bucket
* Browse an S3 bucket
* Upload files to an S3 bucket

## 3. Big Picture
Navigating the AWS console and interacting with AWS services is a key skill for cloud computing.

Similarly, creating users, protecting those users with multi-factor authentication (MFA) and configuring permissions is imperative.

![](https://video.udacity-data.com/topher/2020/June/5edc724f_iam-big-picture/iam-big-picture.png)

## 4. Signing Up With AWS

### Create Your Own AWS Account
Follow these steps to create your own AWS account. You can skip these steps if you already have an AWS account.

* 1. Visit the [Amazon Web Services](https://aws.amazon.com/?nc1=h_ls) homepage
* 2. Click the <strong>Create A Free Account</strong> button
* 3. Provide your email and a strong password, and name your AWS account
* 4. Choose <strong>Personal</strong> account - there is no difference in features or services between a Personal and a Professional account
* 5. Fill in the required fields and click <strong>Continue</strong>
* 6. <strong>Add a payment method.</strong> In this course, we will use services within the [AWS Free Tier](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc), so that you will not be charged. However, the Free Tier has limits and AWS will eventually charge you if you do not terminate your resources. At the end of this course, please remember to delete all the resources you have created.
* 7. Specify a payment method.

### Further Instructions
[Create and Activate an AWS Account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)

## 5. Usage Alerts

The [AWS Free Tier](https://aws.amazon.com/free/) allows you to gain free hands-on experience with AWS service.

The Free Tier has limits, however. AWS does not provide an ability to automatically stop all services before you exceed the Free Tier. However, AWS Usage Alerts can help you monitor if your usage and costs, so that you can stop services yourself before you incur unexpected charges.

AWS Budgets is a service that can be accessed from your root account (or a user with billing admin permissions). This service allows you to create forecasts and alerts to notify you when you are about to exceed your budget.

Specifically, AWS Budgets can monitor your Free Tier usage and notify you via an email alert before you exceed the Free Tier.

* 1. Sign in to the AWS Console with your root account
* 2. Go to [Billing and Cost Managment](https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fbilling%2Fhome%3Fstate%3DhashArgs%2523%26isauthcode%3Dtrue&client_id=arn%3Aaws%3Aiam%3A%3A934814114565%3Auser%2Fportal-aws-auth&forceMobileApp=0&code_challenge=q1YnTQfOB3ZCycHrVI92ijCeezFbxYBqTA3o3uQyVDk&code_challenge_method=SHA-256)
* 3. Under <strong>Preferences</strong>, click on <strong>Billing Preferences</strong> from the left sidebar
* 4. Under <strong>Cost Management Preferences</strong>, select <strong>Receive Free Tier Usage Alerts</strong>

By default, alerts will be sent to the root account email address. If you would like to change that, you can add an alternative address to the <strong>Email address</strong> field.

![](https://video.udacity-data.com/topher/2020/June/5eddd9fc_screen-shot-2020-05-20-at-13.37.34/screen-shot-2020-05-20-at-13.37.34.png)

## 6. Multi-Factor Authentication

### Multi-Factor Authentication (MFA)
* MFA is two-step verification, which increases security
* MFA requires a physical device (such as your smartphone) to generate a code that is matched to your username and password
* Only the correct combination of a username, password, and MFA code allows authentication
* MFA codes refresh every 30 seconds

### Add MFA to Your AWS Account
* Navigate the AWS console to add MFA to your own AWS root account.

## 7. Quiz: Multi-Factor Authentication
### QUIZ QUESTION
How should you secure your AWS root user?
* Set a long and complex password
* Add multi-factor authentication, which requires a physical device to authenticate

## 8. Edge Case: MFA and IAM

### When should you not secure an IAM user with MFA?
Often the cloud can be extended by 3rd party services that are outside the cloud, these 3rd party services providers might not be running on the same cloud provider, thus they need to programmatically log in to AWS.

This login cannot be done with multi-factor authentication as you can't get the 3rd party service provider to physically activate the MFA.

In this situation, you can create a user with AWS credentials and without MFA only grant the minimum permissions needed by the service and rotate the credentials every 30 days

### QUIZ QUESTION
When should you not secure an IAM user with MFA?
* When a 3rd party service needs access to the AWS account

## 9. Securing Root User With MFA

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/13.jpg)](https://www.youtube.com/watch?v=lIRttRwhVQ4&t=25s)

### Securing the Root User with MFA
Multi-factor authentication (MFA) is important and should be activated whenever possible.

You should enable the MFA for the root account.

The Google Authenticator app can scan a QR code from AWS and synchronize with it so that every time you sign in to AWS, you will need to provide a code from Google Authenticator.

## 10. AWS Console

The console is the graphical user interface (GUI) to access and configure AWS services. The AWS console supports both search and navigation. If you have the URL for a service, you can also go directly to that URL (e.g. a bookmark).

The console has built-in help functionality, including wizards and templates to rapidly configure services with default settings.

## 11. Quiz: AWS Console

### QUIZ QUESTION
Name two ways to navigate to an AWS service console.
* Click on the Services dropdown menu
* Use the text field with a magnifying glass to search for a service
* Navigate to the service's URL directly, for example: https://console.aws.amazon.com/apigateway

## 12. IAM

* Identity and Access Management (IAM) is a service that manages access to AWS resources securely
* Policies can be applied to resources or identities
* IAM supports creating users, groups, and roles
* There is no charge for the IAM service
* Access is granted through IAM policies, which are either "built-in", "custom", or "inline"
* IAM policies are usually of the format, "resource:action" (e.g. "s3:ListBucket")

## 13. IAM Users

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/14.jpg)

* An IAM user is an identity that allows access to AWS resources, either via the console (username and password authentication) or programmatically (access key and secret key authentication)
* Users should be granted the least permissions they need - this reduces the potential for error or malfeasance
* Permissions can be attached to the user by built-in policies or by inline policies

## 14. Quiz: Create an IAM User

### QUIZ QUESTION
Which permissions should you grant a user who needs access to read from an S3 bucket but does not need to use any other service?
* Always grant the minimum permissions required

## 15. IAM Policies

* IAM permissions are granted via "policies"
* A policy defines who can access a resource and what actions are allowed on that resource
* Each IAM policy is composed of actions, resources, and principals
>> * principal => either an IAM user or a role
>> * actions => what the principal can / can't do
>> * resources => where can the principal perform these actions

* There are three types of IAM policies:
>> * "Built-in" policies provided by AWS
>> * "Custom" policies created by AWS users
>> * "Inline" policies

![](https://video.udacity-data.com/topher/2020/June/5edd2b78_iam-policy-json/iam-policy-json.png)

## 16. Exercise: Creating A Manager IAM User With Built-in Policies

In this exercise, you will create an IAM user for a manager, and apply built-in IAM policies.

### Instructions
* Create an IAM user
* Name the user "manager"
* Provide this user with:
>> * IAM Full Access permissions
>> * S3 Full Access permissions
>> * EC2 Full Access permissions

## 17. Solution: Creating A Manager IAM User With Built-in Policies

### Creating An IAM User
While logged in as the root account user, navigate to the IAM console.

![](https://video.udacity-data.com/topher/2020/April/5e8b622b_iam-2/iam-2.png)

* 1. From the left sidebar click on <strong>Users</strong> to get into the Users page
* 2. Click the <strong>Add User</strong> button and set the <strong>User name</strong> to <strong>manager</strong>
* 3. Select the <strong>AWS Management Console Access</strong> access type
* 4. Leave the <strong>Autogenerated password</strong> on
* 5. Uncheck the option for <strong>Require password reset</strong>
* 6. Click on the <strong>Next: Permissions</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8b676c_iam-6/iam-6.png)

* 7. Click on the <strong>Attach existing policies directly</strong> button
* 8. Search for <strong>IAMFullAccess</strong> and select it

![](https://video.udacity-data.com/topher/2020/April/5e94a8ab_screen-shot-2020-04-13-at-10.59.09/screen-shot-2020-04-13-at-10.59.09.png)

* 9. Search for <strong>S3FullAccess</strong> and select it

![](https://video.udacity-data.com/topher/2020/April/5e94a8bd_screen-shot-2020-04-13-at-10.59.00/screen-shot-2020-04-13-at-10.59.00.png)

* 10. Search for <strong>EC2FullAccess</strong> and select it

![](https://video.udacity-data.com/topher/2020/April/5e94a818_screen-shot-2020-04-13-at-10.57.05/screen-shot-2020-04-13-at-10.57.05.png)

* 11. Click on the <strong>Next: Tags</strong> button. We don't need to add any tags at the moment, so skip the tags by clicking on the <strong>Next: Review</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e94a8e1_screen-shot-2020-04-13-at-10.57.25/screen-shot-2020-04-13-at-10.57.25.png)

* 12. Click on the Create user button to create the user

![](https://video.udacity-data.com/topher/2020/April/5e8b6a6e_iam-8/iam-8.png)

* 13. Copy and save both the password (show password) and the login URL somewhere you will be able to access it later

## 18. Exercise: Securing IAM User With MFA

In this exercise, you will secure an IAM user with multi-factor authentication (MFA).

### Instructions
* If you have not yet done so, you must first create a <strong>manager</strong> AWS account
* Install an MFA app on your phone - the <strong>Google Authenticator</strong> app ([Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_US), [iOS](https://apps.apple.com/us/app/google-authenticator/id388497605)) is a good choice
* Secure the manager account with MFA
* Log out and log back in to verify that MFA is enabled

## 19. Solution: Securing IAM User With MFA

Navigate to the IAM console and select the user you want to secure with MFA (in this series of exercises this would be the <strong>manager</strong> user). -->9179@82yAnn

* 1. Click on the user account and open the <strong>Security Credentials</strong> tab

![](https://video.udacity-data.com/topher/2020/April/5e8b9d6b_screen-shot-2020-04-06-at-14.19.39/screen-shot-2020-04-06-at-14.19.39.png)

* 2. Click <strong>Manage</strong> next to the <strong>Assign MFA device</strong>
* 3. Leave the default <strong>Virtual MFA device</strong> option on and click continue
* 4. Click the <strong>Show QR code</strong> in the empty square

![](https://video.udacity-data.com/topher/2020/April/5e8ba078_screen-shot-2020-04-06-at-14.34.16/screen-shot-2020-04-06-at-14.34.16.png)

* 5. Open the <strong>Google Authenticator</strong> app on your phone and click the <strong>Scan a barcode</strong> camera icon
* 6. Scan the barcode
* 7. Type the code you see on your phone into the <strong>MFA code 1</strong> field
* 8. Wait for the Google Authenticator app to generate the next code
* 9. Type the next consecutive code into the <strong>MFA code 2</strong> field and click the <strong>Assign MFA</strong> button
* 10. Using a new incognito or private browser window to login with this user and the MFA code from your phone

If you have configured MFA correctly you should be able to log in.

If not:

* 1. Log in as the root user
* 2. Proceed to the IAM service console
* 3. Click on <strong>Users</strong>
* 4. Select the <strong>manager</strong> user
* 5. Visit the <strong>Security credentials</strong> tab
* 6. Next to <strong>Assigned MFA device</strong>, click <strong>Manage</strong>
* 7. Remove the assigned MFA device
* 8. Log out of the root user account
* 9. Log back in with the manager account
* 10. Try again to configure MFA

## 20. Simple Storage Service (S3)

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/15.jpg)

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/16.jpg)

### Simple Storage Service (S3)
* AWS S3 is central cloud object storage available in many geographic locations ("regions")
* Permissions to access S3 are set via AWS IAM policy
* An S3 bucket is an object (file) store with high availability
* Within an S3 bucket, you can create folders and upload files to into specific folders
* S3 storage is very economical
* IAM permissions control access to S3 buckets
* An IAM policy can apply to a specific bucket

## 21. Quiz: S3 Bucket

### QUIZ QUESTION
What is the requirement for uploading to an S3 Bucket ?
* The user must have IAM permissions to write and list files

## 22. Exercise: Creating S3 Bucket And Uploading ContentIn this exercise, you will create an S3 bucket and upload files to it.

### Instructions
* If you have not done so already, register with AWS and authenticate as the manager user
* Create a bucket in the <strong>us-west-2</strong> Oregon region
* Create 2 folders in the bucket: "exercise" and "manager"
* Upload content to both folders (a single file in each folder will suffice)

### Note: Please do not delete the bucket until the end of this course. Deleting a bucket takes a long time. If you delete the bucket and then try to create it again later, you may run into errors.

## 23. Solution: Creating S3 Bucket And Uploading Content

Part-1: Creating The Bucket

* 1. Log out of the root account user by clicking on the top right email next between the Bell icon and the Global dropdown menu
* 2. Log in to the console as the manager, using the information from you've got from the previous step
* 3. Navigate to the S3 console
* 4. Create a new bucket (remember that bucket names are globally unique across all AWS accounts)

![](https://video.udacity-data.com/topher/2020/April/5e8b7269_s3-1/s3-1.png)

Note that if a bucket name already exists you will get a warning.

### Note:

Deleting a bucket takes time, so creating the same bucket name after a deletion would not allow you to create the bucket and will result in a "Bucket already exists error"

![](https://video.udacity-data.com/topher/2020/April/5e8b7268_s3-3/s3-3.png)

* 5. Once the bucket is created, click on the Create folder button to create a manager folder

![](https://video.udacity-data.com/topher/2020/April/5e8b7267_s3-4/s3-4.png)

![](https://video.udacity-data.com/topher/2020/April/5e8b7267_s3-4/s3-4.png)

* 6. Create another folder called exercise

![](https://video.udacity-data.com/topher/2020/April/5e8b73f7_s3-11/s3-11.png)

* 7. Click on the <strong>exercise</strong> folder to get into that folder
* 8. Click on the <strong>Upload</strong> button to upload a file (any file) into that folder

![](https://video.udacity-data.com/topher/2020/April/5e8b7266_s3-5/s3-5.png)

* 9. Either drag and drop a file onto the window or click the Add files button to start the upload process

![](https://video.udacity-data.com/topher/2020/April/5e8b7266_s3-6/s3-6.png)

* 10. Click the <strong>Next</strong> button to see the list of default permissions for this file (we will use IAM permission to access it rather than resource permissions)

* 11. Click Next to see the S3 storage classes, and leave the default Standard class selected

![](https://video.udacity-data.com/topher/2020/April/5e8b7265_s3-7/s3-7.png)

* 12. Click the Upload button to start the upload.

![](https://video.udacity-data.com/topher/2020/April/5e8b7264_s3-8/s3-8.png)

![](https://video.udacity-data.com/topher/2020/April/5e8b7263_s3-9/s3-9.png)

## 24. Exercise: IAM Inline Policy

In this exercise, you will create an IAM user for this specific exercise and apply inline IAM policies.

Creating IAM policies on specific resources requires identifying that specific resource uniquely. AWS uses a unique identifier called an "ARN" (Amazon Resource Name) to identify a specific resource.

### Instructions
* If you have not already done so, sign up with AWS, log in using the <strong>manager</strong> user, create an <strong>S3 bucket</strong>, and create an <strong>exercise</strong> and <strong>manager</strong> folder within that bucket
* As the <strong>manager</strong> user, visit the IAM console and create a new user called <strong>exercise-user</strong>
* Create an <strong>inline IAM policy</strong> on the <strong>exercise-user</strong> allowing:
>> * <strong>ListAllMyBucket:</strong> Required to view the buckets in S3
>> * <strong>ListBucket:</strong> Required to list the contents of a particular bucket - use the <strong>ARN</strong> of the S3 bucket you previously created
>> * <strong>GetObject:</strong> Required to view any object within the <strong>exercise</strong> folder - use <strong>ARN (Amazon Resource Name)</strong> of the folder
>> >> * The <strong>ARN</strong> of the folder is in the format: "[bucket_name]/[folder_name]" (e.g. "udacity/exercise")

![](https://video.udacity-data.com/topher/2020/June/5edd3aa2_iam-inline-policy/iam-inline-policy.png)

## 25. Solution: IAM Inline Policy

While logged in as the <strong>manager</strong> user account via an incognito/private browser window, create the <strong>exercise</strong>IAM user as follow:

* 1. Navigate to the IAM console
* 2. From the left sidebar menu, click on Users
* 3. Click on <strong>Add user</strong> button and name it <strong>exercise-user</strong>
* 4. Select the option <strong>AWS Management Console access</strong> and uncheck the <strong>Require password reset</strong> option
* 5. Skip the <strong>Set permissions</strong> and create the user by clicking through the <strong>Next</strong> button
* 6. Note the password for the <strong>exercise</strong> user and click the <strong>Close</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8b784e_iam-9/iam-9.png)

## Granting Permissions For The Exercise User
In order for the <strong>exercise</strong> user to be able to download/upload content on the S3 bucket we need the following permissions:

<strong>ListAllMyBuckets</strong> - allow listing all the buckets in the console <strong>ListBucket</strong> - allow listing a specific bucket content <strong>GetObject</strong> - allow retrieving a file

<strong>Note:</strong> for upload permission we would need the <strong>PutObject</strong> permission (this is not a requirement for this exercise)

### Creating an IAM Inline Policy
* 1. Click the <strong>exercise</strong> user to get into the user details
* 2. Click the <strong>+ Add inline policy</strong> link to create a new policy

![](https://video.udacity-data.com/topher/2020/April/5e8b794a_iam-policy-1/iam-policy-1.png)

* 3. In the <strong>Service</strong> field Select <strong>S3</strong>
* 4. Type <strong>ListBucket</strong> in the <strong>Actions</strong> field and select <strong>ListBucket</strong> as well as <strong>ListAllMyBuckets</strong>

![](https://video.udacity-data.com/topher/2020/April/5e8b8508_s3-13/s3-13.png)

* 5. Under the <strong>Resources</strong> dropdown, select <strong><Specific</strong> and set the bucket name to the bucket name you have created previously

![](https://video.udacity-data.com/topher/2020/April/5e8b96eb_screen-shot-2020-04-06-at-13.53.25/screen-shot-2020-04-06-at-13.53.25.png)

![](https://video.udacity-data.com/topher/2020/April/5e8b7a2f_ima-policy-5/ima-policy-5.png)

### Read-Only (GetObject) Permissions
* 1. Click the <strong>Add additional permissions</strong> link
* 2. Select <strong>S3</strong>at the <strong>Service</strong> field and type <strong>GetObject</strong> in the <strong>Actions</strong> field
* 3. Select the <strong>GetObject</strong> option
* 4. Now let's limit the user access to the <strong>exercise</strong> folder, expand the <strong>Resources</strong> section and click on <strong>Add ARN</strong> link
* 5. Fill in the bucket name and in the object field type the folder name <strong>exercise</strong>
* 6. Since objects are just files and not folder the bucket name will hold the folder name to access, so click on the <strong>Any</strong> checkbox to grant read on any object in the <strong>exercise</strong> folder

![](https://video.udacity-data.com/topher/2020/April/5e8b7c7a_iam-policy-8/iam-policy-8.png)

* 7. Name the policy <strong>exerciseReadOnlyAccess</strong> and create it

![](https://video.udacity-data.com/topher/2020/April/5e8b7d27_iam-policy-10/iam-policy-10.png)

### Part-2: Validation
* 1. Using the <strong>exercise</strong> user in a new incognito/private browser window log in to the AWS console
* 2. Navigate to the S3 bucket and click on the bucket you have created
* 3. You should be able to see both folders <strong>manager</strong> and <strong>exercise</strong> - you should only be able to download any file from the exercise folder and none from the manager folder
* 4. Click on the <strong>exercise</strong> folder and select a file, try to delete it from the <strong>Actions</strong> button and verify you get a <srong>permission denied</strong> error

![](https://video.udacity-data.com/topher/2020/April/5e8b982f_screen-shot-2020-04-06-at-13.09.35/screen-shot-2020-04-06-at-13.09.35.png)

## 26. Quiz: Read-Only IAM Policy

### Quiz: Read-Only IAM Policy

### QUESTION 1 OF 2
What is the name of the service to create users and access policies?

* IAM

### QUESTION 2 OF 2
Which of the following permissions are read-only?
* "S3:ListBucket"

* "S3:GetObject"

## 27. Lesson Conclusion

### Lesson Recap
In this lesson you:

* Signed up for AWS
* Created multiple IAM users
* Secured those users with multi-factor authentication
* Attached IAM policies to those users
* Navigated AWS services using the console
* Created an S3 bucket
* Browsed, uploaded to, and downloaded from that S3 bucket

In the next lesson, you will:

* Learn about the Elastic Compute Cloud (EC2) service
* Launch an EC2 instance (i.e. a virtual server)
* Configure security groups to control access to that instance
* Allocate a static IP via Elastic IP
* Provision the instance via an init script
* Create an IAM role to manage the EC2 instance
* Connect your EC2 and S3 resources

Let's go!

![](https://video.udacity-data.com/topher/2020/June/5edc6f1b_course-outline/course-outline.png)

### Further Reading
### Documentation
* IAM Getting Started (https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html)
* Understanding how IAM works (https://docs.aws.amazon.com/IAM/latest/UserGuide/intro-structure.html)
* IAM policy evaluation logic (https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_evaluation-logic.html)
* Testing IAM Policies with the IAM policy simulator (https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_testing-policies.html)

### Blogs
* Demystifiying AWS IAM (https://blog.getdockup.com/post/demystifying-aws-iam/)
* AWS IAM Deep Dive (https://blog.tovmasyan.io/aws-iam-deep-dive-chapter-1-essentials-a9cfb1931a01?gi=a033437d2647)
* AWS IAM Resources (https://aws.amazon.com/iam/resources/?nc=sn&loc=4&iam-blogs.sort-by=item.additionalFields.createdDate&iam-blogs.sort-order=desc)

## 28. Glossary

* <strong>Bucket:</strong> a storage resource within S3, similar to a folder

* <strong>IAM:</strong> Identity and Access Management is the service for creating identities and policies to govern access to resources

* <strong>IAM User:</strong> a type of identity designed for console and programmatic access to the AWS services

* <strong>IAM Policy:</strong> a document defining who can do what on which resource

* <strong>Object:</strong> a unit of storage in S3, typically an object is a file

< strong>S3:</strong> Simple Storage Service, which is AWS's service to store files in the cloud

## 29. AWS Account Setup

### Step 1. Create an AWS Account
Open a regular AWS account (if you don't already have one) following the instructions via the [Amazon Web Service Help Center](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)

### Step 2. Get Promo Codes
Udacity has partnered with AWS to provide nominal credits for learners whose coursework requires AWS services to complete. To request a promo code, you can submit a Support ticket [here](https://udacity.zendesk.com/hc/en-us/signin?return_to=https%3A%2F%2Fudacity.zendesk.com%2Fhc%2Fen-us%2Frequests%2Fnew%3Fticket_form_id%3D110806).

* 1. Under the <strong>"Reason for Contact"</strong> field, choose <strong>"Third-Party Access, Promo Codes & License keys"</strong>, then choose <strong>"AWS"</strong> in the dropdown.

![](https://video.udacity-data.com/topher/2020/November/5fbb4c2e_screenshot-2020-11-23-at-11.13.32-am/screenshot-2020-11-23-at-11.13.32-am.png)

* 2. Please note that a regular AWS account will receive a promo code from Udacity with a fixed amount of AWS credits.

### Step 3. Apply Promo Code to Your AWS Account
To apply your promo code, follow below:

* 1. Go to the [AWS Billing Dashboard](https://us-east-1.signin.aws.amazon.com/oauth?response_type=code&client_id=arn%3Aaws%3Aiam%3A%3A934814114565%3Auser%2Fportal-aws-auth&redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fbilling%2Fhome%3Fstate%3DhashArgs%2523%252F%26isauthcode%3Dtrue&forceMobileLayout=0&forceMobileApp=0&code_challenge=dkR7DMIVwTgADA6smwewYbv8YS-T1FQlFO0UBBIQi7Q&code_challenge_method=SHA-256).
* 2. Click <strong>"Credits"</strong> on the left side of the screen, and click on the <strong>Redeem credit</strong> button. Enter the promo-code you have received.
* 3. Credits will automatically be applied to your bill. Refresh the page and you will be able to view your credits under the <strong>Credits</strong> page.

![](https://video.udacity-data.com/topher/2020/November/5fbb4a3b_screenshot-2020-11-23-at-11.02.59-am/screenshot-2020-11-23-at-11.02.59-am.png)

### AWS Free Tier
It is an offering from AWS that allows you to use most of the AWS services free of cost up to a certain usage limit for one year. In addition to the promo codes provided by Udacity, you can also leverage the [AWS Free Tier Access](https://aws.amazon.com/premiumsupport/knowledge-center/what-is-free-tier/).

### According to AWS:

>>> The AWS Free Tier is automatically activated on each new AWS account.

Check the list of services covered under Free Tier [here](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all).

>> <strong>Note</strong> - You will be responsible for charges incurred from usage that exceeds the AWS Free Tier limits and credits provided by Udacity.

## 30. Monitor your AWS Costs and Credits

### Monitoring your AWS Costs and Credits
All AWS services are a pay-as-you-go service, so we urge our students to closely monitor their usage costs and if they have adequate credits available to complete their project/task. Follow the instructions below to do that:

### Step 1. Log into your [AWS account](https://us-east-1.signin.aws.amazon.com/oauth?SignatureVersion=4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJMOATPLHVSJ563XQ&X-Amz-Date=2021-04-06T05%3A57%3A42.069Z&X-Amz-Signature=02894049d5815ce76e8fb52cd7d554973ff2c87bf57e93f3d2bb1625ef8c2023&X-Amz-SignedHeaders=host&client_id=arn%3Aaws%3Aiam%3A%3A015428540659%3Auser%2Fhomepage&code_challenge=0pDPeSFi-xicamChdPUR7H4Yk9fG2pEhgnn8lzyDUp4&code_challenge_method=SHA-256&redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fconsole%2Fhome%3Fstate%3DhashArgs%2523%26isauthcode%3Dtrue&response_type=code&state=hashArgs%23).
### Step 2. Examine your costs
Go to [https://console.aws.amazon.com/billing/](https://us-east-1.signin.aws.amazon.com/oauth?SignatureVersion=4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAI6EECTLVZXJOHYRQ&X-Amz-Date=2021-04-06T05%3A58%3A09.860Z&X-Amz-Signature=edbf1e40599fd2c7f506e6a5cb075b956365fd8953895a646fc9cf80cdba5120&X-Amz-SignedHeaders=host&client_id=arn%3Aaws%3Aiam%3A%3A934814114565%3Auser%2Fportal-aws-auth&code_challenge=VWbOI_OMsEtleqMelhpx-TbkI53XyRgimyaPteyhquE&code_challenge_method=SHA-256&redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fbilling%2Fhome%3Fstate%3DhashArgs%2523%26isauthcode%3Dtrue&response_type=code&state=hashArgs%23)

You should see the following billing dashboard where it will show your costs.

![](https://video.udacity-data.com/topher/2020/May/5ec71862_screen-shot-2020-05-21-at-5.07.48-pm/screen-shot-2020-05-21-at-5.07.48-pm.png)

If your account has been created within one year from the current date, your [AWS Billing Dashboard](https://us-east-1.signin.aws.amazon.com/oauth?SignatureVersion=4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAI6EECTLVZXJOHYRQ&X-Amz-Date=2021-04-06T05%3A59%3A24.703Z&X-Amz-Signature=6e5319b643c4627cec8895c59cfb7268a2b017a1cd534e578780128c6a6c61ee&X-Amz-SignedHeaders=host&client_id=arn%3Aaws%3Aiam%3A%3A934814114565%3Auser%2Fportal-aws-auth&code_challenge=wWhT_Fk_BVY_1NvSP7ZnIC71MVSh0OjNbOood6I6xt4&code_challenge_method=SHA-256&redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fbilling%2Fhome%3Fstate%3DhashArgs%2523%252F%26isauthcode%3Dtrue&response_type=code&state=hashArgs%23%2F) will also show the resource usage statistics for the free tier services. See the snapshot below:

![](https://video.udacity-data.com/topher/2020/November/5fbb70d9_screenshot-2020-11-23-at-12.54.53-pm/screenshot-2020-11-23-at-12.54.53-pm.png)

### Step 3 (optional). Check the value of your credits.
Click on the "Credits" from the left navigation menu, and the following screen will show your available credits.

![](https://video.udacity-data.com/topher/2020/May/5ec71a62_screen-shot-2020-05-21-at-5.13.56-pm/screen-shot-2020-05-21-at-5.13.56-pm.png)

### Note: For student learning, Udacity has partnered with Amazon to provide nominal credits for the student to complete their course work. Please understand that these credits are limited and available for you to use judiciously. You are responsible for any additional costs beyond the given credits.

### When will I be charged?
There are no tools to limit usage to what’s covered by the AWS Free Tier. This means that you are responsible for the services that you launch. You will be charged standard pay-as-you-go service rates for using AWS resources that exceed the AWS Free Tier limits and the credits provided by Udacity.

### Shut Down your Resources, if not in use
>> The Free Tier benefits and the credit amount provided by the Udacity Support team will be sufficient for you to complete your Nanodegree program.

>> <strong>Note:</strong> We recommend you shut down every resource (e.g., EC2 instances, or any other hosted service) on the AWS cloud immediately after the usage, otherwise you will run out of your free promo credits.

Remember, even if you are in the middle of the project and need to step away, PLEASE SHUT DOWN YOUR RESOURCES. You can re-instantiate later.

________________________________________________________________________________________________________________________________________________________________________________

# LESSON 4 COMPUTE SERVICES

## 1. Compute Services

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/17.jpg)

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/18.jpg)

### Compute Services
### Regions and Availability Zones
AWS EC2 is available worldwide, in geographical areas called "regions". Each region contains between 2 and 6 data centers sited miles away from each other and connected to their own power and networking.

Each of those data centers is called an “availability zone”. Within a region, the availability zones are interconnected with fiber-optic cables or other ultra-fast connections.

### Instance types
EC2 has a wide selection of instance types optimized to fit different use cases. An instance type is comprised of CPU, memory, storage, and networking. The range of instance types EC2 offers gives you the flexibility to choose the right mix for your application.

### Auto Provisioning
In the cloud, servers can scale up automatically. Launching and configuring an instance automatically, without human intervention, is crucial for smooth and reliable operation. Launching and configuring each instance manually is a recipe for human error.

EC2 allows you to run a custom script the first time an instance boots, for just this reason.

### Security Groups
Security is very important in the cloud. Access to servers is enforced with firewall rules knowns as “security groups”.

### Elastic IP Address
Instances' public IP addresses are dynamic and will change when you restart your instance, An Elastic IP Address is static and can always remain attached to the instance you want. An Elastic IP is public and reachable from the Internet.

Throughout this lesson you will practice working with all of these core features of AWS EC2.

![](https://video.udacity-data.com/topher/2020/June/5edd8999_amazon-ec24x/amazon-ec24x.png)

## 2. Lesson Outline

### Course Outline
In this lesson, you will:

* Create an EC2 instance
* Automatically provision that instance
* Configure a security group to allow incoming HTTP connections
* Connect your EC2 instance with your existing S3 bucket, via IAM roles and policies

In future lessons, you will:

* Create databases
* Program a serverless function

![](https://video.udacity-data.com/topher/2020/June/5edc6f1b_course-outline/course-outline.png)

### Lesson Outline
This lesson covers launching an EC2 instance, configuring automatic provisioning via an init script, creating security groups (i.e. a firewall) to allow incoming HTTP connections, and connecting the EC2 instance with an S3 bucket via an IAM role.

### Learning Objectives
In this lesson, you will:

* Create an IAM role for an EC2 instance
* Configure a read-only inline IAM policy to access an S3 bucket
* Launch a Linux virtual machine (EC2 instance)
* Create a security group to allow HTTP access on port 80
*  Attach an Elastic IP address to an EC2 instance
* Create an init script to install the NGINX webserver on your instance
* Terminate an EC2 instance
* Update the init script to replace the default NGINX webpage with content from your s3 bucket
* Launch a new EC2 instance that automatically pulls your custom webpage from S3

## 3. Big Picture

### Big Picture
EC2 is the heart of AWS cloud computing, and was the very first compute service that AWS offered, starting in 2006. There are now many compute services on AWS, but EC2 remains the most important.

Automation and security best practices are critical when connecting EC2 to other AWS services, in order to minimize human error and create a path for automatic scaling in the future.

That why, in this lesson, you'll practice not only launching EC2 instances, but also configuring security and provisioning the instances automatically.

![](https://video.udacity-data.com/topher/2020/June/5edd9192_ec2-big-picture/ec2-big-picture.png)

## 4. Launching An EC2 Instance

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=WxigbPUJCd0&t=3s)

### AWS Elastic Compute Cloud (EC2)
* Resizeable, scalable compute capacity
* Instances sizes are predefined by instance types
* Configuring an instance can be done within the EC2 Launch Wizard:
* Security groups (i.e. firewall rules)
* Networking (public or private)
* Storage size and type
* Custom provisioning scripts

## 5. Quiz: EC2 Instances

### QUESTION 1 OF 2
How do you terminate an EC2 Instance from the AWS Console?
* Select the Instance and then select Actions -> Instance State -> Terminate

### QUESTION 2 OF 2
In which section would you enlarge the instance's attached hard drive?
* Add Storage

## 6. Exercise: Launch An E2 Instance

In this exercise, you will launch an EC2 instance.

No need to connect to this instance using a key pair.

### Instructions
* Region: <strong>us-east-1</strong>
* AMI: <strong>Amazon Linux 2 AMI (HVM), SSD Volume Type 64-bit</strong>
* Type: strong>t2.micro</strong> (Free Tier = 750 hours per month)
* Root volume size: <strong>20GB</strong>
* IP: <strong>Public</strong>

## 7. Solution: Launch An E2 Instance

### Solution: Launch An EC2 Instance
Use the <strong>us-east-1 N.Vriginia</strong> region to launch an EC2 instance with the following configuration:

* <strong>AMI:</strong> Amazon Linux
* <strong>Instance type:</strong> t2.micro
* <strong>IP:</strong> Public
* <strong>Storage size:</strong> 20GB

For this exercise, we can skip the creation of a new key pair, and acknowledge that we will not be able to connect to the instance.

![](https://video.udacity-data.com/topher/2020/April/5e8cb98d_screen-shot-2020-04-07-at-10.33.54/screen-shot-2020-04-07-at-10.33.54.png)

Choose the <strong>Amazon Linux 2 AMI (HVM), SSD Volume Type 64-bit</strong> image.

![](https://video.udacity-data.com/topher/2020/April/5e8cba04_screen-shot-2020-04-07-at-10.35.25/screen-shot-2020-04-07-at-10.35.25.png)

Select the <strong>t2.micro</strong> option and click the <strong>Next: Configure Instance Details</strong> button.

![](https://video.udacity-data.com/topher/2020/April/5e8cbde0_screen-shot-2020-04-07-at-10.51.46/screen-shot-2020-04-07-at-10.51.46.png)

* 1. Skip the defaults for VPC and Subnet
* 2. Change the <strong>Auto-assign Public IP</strong> field from the default <strong>disabled</strong> to <strong>Enable</strong> and then click <strong>Next: Add Storage</strong> button
* 3. Change the default size from <strong>8GB</strong> to <strong>20GB</strong>

![](https://video.udacity-data.com/topher/2020/April/5e8cbcae_screen-shot-2020-04-07-at-10.47.15/screen-shot-2020-04-07-at-10.47.15.png)

Since we do not need any further configuration we can click on the <strong>Review and Launch</strong> button.

![](https://video.udacity-data.com/topher/2020/April/5e8ce73f_screen-shot-2020-04-07-at-13.42.26/screen-shot-2020-04-07-at-13.42.26.png)

Choose to proceed without an SSH key pair.

![](https://video.udacity-data.com/topher/2020/April/5e8ce859_screen-shot-2020-04-07-at-13.52.24/screen-shot-2020-04-07-at-13.52.24.png)

For this exercise, we can skip the creation of a new key pair, and acknowledge that we will not be able to connect to the instance.

![](https://video.udacity-data.com/topher/2020/April/5e8ce916_screen-shot-2020-04-07-at-13.55.50/screen-shot-2020-04-07-at-13.55.50.png)

Select <strong>Proceed without a key pair</strong> and check the box for <strong>I acknowledge that....</strong> Then click on the <strong>Launch Instances</strong> button.

![](https://video.udacity-data.com/topher/2020/April/5e8ce9b4_screen-shot-2020-04-07-at-13.58.09/screen-shot-2020-04-07-at-13.58.09.png)

Every instance has an ID. If we click on the ID starting with the prefix i- we can see the instance.

![](https://video.udacity-data.com/topher/2020/April/5e8cea47_screen-shot-2020-04-07-at-14.00.46/screen-shot-2020-04-07-at-14.00.46.png)

In this page we can verify that:

* Our instance type is: <strong>t2.micro</strong>
* An <strong>IPv4 Public IP</strong> has been allocated
* The instance is <strong>running</strong>
>> * The instance may first take several minutes to boot

## 8. Security Group

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=zn-TVaoy9KE&t=150s)

### Security Group
* Acts as a firewall
* Ingress rules can be added to allow traffic to specific services and ports
* Security groups are scoped to an instance level, not to a network or subnet
* You can specify ALLOW rules but you can't specify DENY rules
* You can control traffic via an IP address range (CIDR), or via security group IDs (for other AWS resources)

## 9. Quiz: Security Group

### QUIZ QUESTION
What is the purpose of an AWS security group?
* Control inbound and outbound traffic

## 10. Exercise: Security Group
In this exercise, you will create a <strong>security group</strong> to allow traffic to an instance.

### Instructions
* If you have not done so already, launch an EC2 instance
* Create a new Security Group allowing <strong>Port 80</strong> and <strong>Port 22</strong> Inbound traffic from <strong>anywhere</strong> (any IP address)
* Attach the security group to the instance

## 11. Solution: Security Group

### Solution: Security Group Exercise
If you have not done so already, launch an EC2 instance from the EC2 console.

### Part 1: Create a Security Group
From the EC2 console, scan the sidebar to find the <strong>Network & Security</strong> section. Within that section click on <strong>Security Groups</strong>.

![](https://video.udacity-data.com/topher/2020/April/5e8cf604_screen-shot-2020-04-07-at-14/screen-shot-2020-04-07-at-14.jpg)

Click on the <strong>Create security group</strong> button

Fill the information for your security group name and description.

![](https://video.udacity-data.com/topher/2020/April/5e8cf70f_screen-shot-2020-04-07-at-14.55.06/screen-shot-2020-04-07-at-14.55.06.png)

Click on the <strong>Add Rule</strong> button under the inbound section and add the following rules:

```
SSH TCP 22 Anywhere

HTTP TCP 80 Anywhere
```
![](https://video.udacity-data.com/topher/2020/April/5e8cf7ba_screen-shot-2020-04-07-at-14.58.59/screen-shot-2020-04-07-at-14.58.59.png)

Click on the <strong>Create security group</strong> button to create the security group.

<strong>Part 2: Attach The Security Group To An EC2 Instance</strong>
Navigate via the sidebar to EC2 Instances Dashboard. Select the instance to which you want to add the security group.

From the <strong>Actions</strong> dropdown menu select <strong>Networking</strong>, followed by <strong>Change Security Groups</strong>.

![](https://video.udacity-data.com/topher/2020/April/5e8cfd23_screen-shot-2020-04-07-at-15.20.11/screen-shot-2020-04-07-at-15.20.11.png)

Select the security group you just created in Step 1 and click the <strong>Assign security groups</strong> button.

In the <strong>Description</strong> tab at the bottom of the screen, we can now see the security group.

![](https://video.udacity-data.com/topher/2020/April/5e8cfdfa_screen-shot-2020-04-07-at-15.24.37/screen-shot-2020-04-07-at-15.24.37.png)

## 12. Terminate Instance

Now that you have practiced launching an EC2 instance, let's practice cleaning up (i.e. terminating) that instance. Cleaning up resources is important so that we don't incur any unexpected charges.

Select the instance ID from the AWS Instances console.

![](https://video.udacity-data.com/topher/2020/June/5edd9a73_select-instance/select-instance.png)

From the <strong>Actions</strong> dropdown menu, select <strong>Instance State</strong>, followed by <strong>Terminate</strong>.

![](https://video.udacity-data.com/topher/2020/June/5edd9ac0_terminate-instance/terminate-instance.png)

Confirm that the instances reaches the <strong>Terminated</strong> state. This may take a few minutes.

## 13. Init Script

### Init Script
* An init script can be configured on instance launch page under userData section
* Can be used to run commands, install and configure an instance only during first boot
* Can be configured to run on every reboot
* Instances must have a public IP to install software from the internet
* Can be written in any language if the instance image AMI has the required software, mainly written in Bash

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=E3J73eQqopo&t=1s)

## 14. Quiz: Init Script

### QUESTION 1 OF 3
Which of the following are true about init scripts?

* Automatically install and configure software
* Launch the first time an instance boots
* Can be launched on every reboot - if so configured

### QUESTION 2 OF 3
Where in the EC2 Launch Wizard do we add an init script?
* User Data section

### QUESTION 3 OF 3
What is the default behavior for an init script configuration?
* An init script only runs the first time an instance boots

## 15. Exercise: Init Script
In this exercise, you will automatically provision an EC2 Instance using an init script, which runs at first boot.

### Instructions
* EC2 instance AMI: <strong>Amazon Linux AMI 2</strong>
* Instance type: <strong>t2.micro</strong>
* Instance should be open for traffic from <strong>anywhere</strong> on <strong>port 80</strong>
* Instance must have a <strong>public IP address</strong> to be able to reach the internet and install <strong>NGINX</strong>

For this exercise, we can ignore SSH permissions, as we do not need them.

Use this code as the init-script:

```
  #!/bin/bash

  yum update -y
  amazon-linux-extras install nginx1.12 -y
  service nginx start
```

### Goal
We should be able to access the instance's public IP address via a web browser. The NGINX default page should appear: <strong>Welcome to NGINX</strong>.

## 16. Solution: Init Script Exercise

### Solution: Init Script Exercise
When you launch an EC2 instance, you have the option of passing <strong>user-data</strong> that you can use to configure or install software on your instance.

This is also known as an "Init script". For this exercise solution, we will program a shell script to be our init script.

By default, Init scripts run only on the first boot of the instance. We can configure an existing instance to run its init script on every restart, but we do not need that for this exercise.

### Part 0: Clean Up
If you haven't already, terminate all previous instances by selecting them in the EC2 Instances Dashboard. From the <strong>Actions</strong> dropdown menu select <strong>Instance state</strong>, followed by <strong>Terminate</strong>.

![](https://video.udacity-data.com/topher/2020/April/5e8cebfc_screen-shot-2020-04-07-at-14.08.47/screen-shot-2020-04-07-at-14.08.47.png)

### Part :1 Launch an EC2 Instance
* 1. Using the EC2 Console, select Instances from the sidebar and click <strong>Launch instance</strong>
* 2. Select <strong>t2.micro</strong> instance type and click the <strong>Next: Configure Instance Details</strong> button
* 3. Set the <strong>Auto-assign public IP</strong> to <strong>Enabled</strong>, because we need an Internet connection to install the NGINX software
* 4. Scroll down to the <strong>Advanced Details</strong> section, where we will configure the init script to install the NGINX server

![](https://video.udacity-data.com/topher/2020/April/5e8d24cc_screen-shot-2020-04-07-at-18.10.33/screen-shot-2020-04-07-at-18.10.33.png)

5. Copy the following commands into the <strong>User data</strong> box

```
#!/bin/bash

yum update -y
amazon-linux-extras install nginx1.12 -y
service nginx start
```

* 6. Click <strong>Review and Launch</strong>, then edit the <strong>Security Groups</strong>
* 7. Either select an existing security group that allows HTTP access, or create a new such security group
* 8. Click <strong>Review and Launch</strong> and then launch the EC2 instance
* 9. Find the instance's <strong>IPv4 Public IP</strong> address from the EC2 Instance Dashboard
* 10. Visit the IP address in the browser and you should see the default Nginx page

![](https://video.udacity-data.com/topher/2020/April/5e8d29fc_screen-shot-2020-04-07-at-18.29.41/screen-shot-2020-04-07-at-18.29.41.png)

## 17. Elastic IP

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/20.jpg)
![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/21.jpg)
![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/22.jpg)

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=P4c5bS6jpBw)

### Elastic IP
* Allocate a public, static IP address that can be associated with an instance
* Reachable from the internet
* Once associated, it becomes the public IP of the instance
* You can not have 2 public IP address per instance
* Can be disassociated from an instance
* You only pay for unassociated Elastic IPs

## 18. Quiz: Elastic IP

### QUIZ QUESTION
What is the purpose of creating an Elastic IP Address?
* To reserve a static IP address that can be attached to an AWS resource

## 19. Exercise: Elastic IP

In this exercise, you will allocate an Elastic IP and assign it to your instance.

### Instructions
* If you have not done so already, launch an EC2 instance
* Allocate an <strong>Elastic IP</strong>
* Associate the Elastic IP with your EC2 instance
* Verify that the Elastic IP address works

## 20. Solution: Elastic IP

By default, EC2 instances do not get a public IP address. Even If you do assign an automatic public IP address in the Launch Wizard, the address will change on the next restart.

Elastic IP is a way to maintain the same external public IP address for an Instance or application.

From the EC2 console sidebar menu, under the <strong>Network & Security</strong> section click on <strong>Elastic IPs</strong> .

![](https://video.udacity-data.com/topher/2020/April/5e8d016d_screen-shot-2020-04-07-at-15.38.06/screen-shot-2020-04-07-at-15.38.06.png)

Click on the <strong>Allocate Elastic IP Address</strong> button to allocate a new IP address out of the AWS IPv4 pool.

![](https://video.udacity-data.com/topher/2020/April/5e8d017a_screen-shot-2020-04-07-at-15.38.47/screen-shot-2020-04-07-at-15.38.47.png)

Click on the <strong>Allocate</strong> button.

![](https://video.udacity-data.com/topher/2020/April/5e8d018e_screen-shot-2020-04-07-at-15.39.10/screen-shot-2020-04-07-at-15.39.10.png)

The newly-created Elastic IP address is not associated with any instance. Click on the <strong>Associate this Elastic IP address</strong> button, or select it and from the <strong>Actions</strong> dropdown and choose <strong>Associate Elastic IP Address</strong>.

In the next window, in the instance field, select the instance with which you want to associate the Elastic IP address.

![](https://video.udacity-data.com/topher/2020/April/5e8d02f3_screen-shot-2020-04-07-at-15.39.31/screen-shot-2020-04-07-at-15.39.31.png)

![](https://video.udacity-data.com/topher/2020/April/5e8d02dc_screen-shot-2020-04-07-at-15.39.47/screen-shot-2020-04-07-at-15.39.47.png)

Once the instance is associated, you can click on <strong>Associated Instance ID</strong> to see the instance's details. On that screen, you can see the Elastic IP next to the instance ID. You can also verify that the Elastic IP address is the same as the instance's IPv4 Public IP.

![](https://video.udacity-data.com/topher/2020/April/5e8d01a0_screen-shot-2020-04-07-at-15.40.19/screen-shot-2020-04-07-at-15.40.19.png)

## 21. IAM Role

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=8s6W9YfgjuA&t=181s)

### IAM Role
* An IAM identity that does not have long-term credentials
* Can be assumed by a trusted service and operate on your behalf
* Designed for service-to-service communication
* Defines a set of permissions for accessing AWS services
* Is not bound to an identifiable user

![](https://video.udacity-data.com/topher/2020/June/5eddcabb_iam-role/iam-role.png)

## 22. Quiz: IAM Role

### QUIZ QUESTION
What is the difference between an IAM user and an IAM role?
* IAM user has long-term credentials while IAM role does not have credentials

## 23. Exercise: IAM Role

In this exercise, you will create an IAM role with a read-only policy to an S3 bucket.

### Instructions
* If you have not already done so, create an S3 bucket with a folder inside
* Create an IAM Role
* Attach an <strong>Inline IAM Policy</strong> allowing <strong>Read-Only</strong> access to that <strong>S3 bucket</strong>

## 24. Solution: IAM Role Exercise

An IAM Role is an IAM identity similar to IAM user. Instead of uniquely associating with a person, a role is designed for anyone who needs to assume it. This is an excellent fit for a service or a server-to-server identity.

A role is more secure than the long-lived credentials of an IAM user because when the role is assumed it provides temporary security credentials that expire and renew every 15 minutes

### Create the IAM Role
* Navigate to the <strong>IAM console</strong>
* Click <strong>Roles</strong> on the sidebar menu
* Click on the <strong>Create Role</strong> button
* Since we intended to use the role on an EC2 in the next exercise, choose <strong>EC2</strong> as the use case, and click on <strong>Next: Permissions</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8e1491_screen-shot-2020-04-08-at-11.03.54/screen-shot-2020-04-08-at-11.03.54.png)

* 5. If we were to click on the <strong>Create</strong> Policy button, the role creation would be canceled, so instead click on Next until you get to the review page
* 6. Name the role <strong>web</strong> and click on the <strong>Create Role</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8e1497_screen-shot-2020-04-08-at-11.14.34/screen-shot-2020-04-08-at-11.14.34.png)

![](https://video.udacity-data.com/topher/2020/April/5e8e14fc_screen-shot-2020-04-08-at-11.16.17/screen-shot-2020-04-08-at-11.16.17.png)

### Creating and Attaching an IAM Policy to the Role
Now that we have a role, let's create an IAM policy so that it can access our S3 bucket.

* 1. From the sidebar menu click on <strong>Policies</strong> and then click on the <strong>Create Policy</strong> button
* 2. Select <strong>S3</strong> for the service
* 3. On the <strong>Actions</strong> field select <strong>ListBucket</strong> and <strong>GetObject</strong>
* 4. Click on Resources, while it is set to <strong>specific</strong> click the <strong>Add ARN</strong> for the <strong>bucket</strong> and add your bucket name
* 5. Click on the <strong>Add ARN</strong> for the object, set the <strong>bucket name</strong> again to your bucket name and set the <strong>object name</strong> to "web/*"

![](https://video.udacity-data.com/topher/2020/April/5e8e1c1b_screen-shot-2020-04-08-at-11.45.42/screen-shot-2020-04-08-at-11.45.42.png)

![](https://video.udacity-data.com/topher/2020/April/5e8e44db_screen-shot-2020-04-08-at-14.35.20/screen-shot-2020-04-08-at-14.35.20.png)

* 7. Click on the <strong>Review policy</strong> button, set a name (for example, "ec2_web_s3_access") and click the <strong>Create policy</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8e1cc9_screen-shot-2020-04-08-at-11.49.37/screen-shot-2020-04-08-at-11.49.37.png)

### Attaching the Policy to the IAM Role
* 1. Click on the <strong>Roles</strong> on the sidebar menu of the IAM console
* 2. Search for the role "web"

![](https://video.udacity-data.com/topher/2020/April/5e8e1d29_screen-shot-2020-04-08-at-11.51.08/screen-shot-2020-04-08-at-11.51.08.png)

* 3. Click on the role name to edit the role
* 4. Click on the <strong>Attach policies</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8e1dff_screen-shot-2020-04-08-at-11.52.53/screen-shot-2020-04-08-at-11.52.53.png)

* 5. Search for "web" to find the policy you just created
* 6. Select it and click the <strong>Attach policies</strong> button

![](https://video.udacity-data.com/topher/2020/April/5e8e1e75_screen-shot-2020-04-08-at-11.56.43/screen-shot-2020-04-08-at-11.56.43.png)

## 25. Overriding NGINX Defaults

### Overriding NGINX Defaults
NGINX comes with a default web page to verify that the webserver is working.

Instead of configuring a new site for NGINX, we can copy a website to this default location. Our new website will replace the existing NGINX default.

We will store this content in an S3 bucket under the <strong>web</strong> folder. In order to access this content, the following prerequisite must exist:

* S3 bucket storing the zip file for the [SB Admin 2](https://startbootstrap.com/theme/sb-admin-2) theme
* IAM role and policy for EC2 to access the bucket

### Provisioning Script
### Note: Make sure to change "BUCKET_NAME" to the name of the bucket you created

```
#!/bin/bash

   BUCKET_NAME=<s3-bucket-name-place-holder>
   yum update -y
   amazon-linux-extras install nginx1.12 -y
   service nginx start
   aws s3 cp s3://${BUCKET_NAME}/web/startbootstrap-sb-admin-2-gh-pages.zip /tmp/
   cd /tmp
   unzip start*
   mv startbootstrap-sb-admin-2-gh-pages html
   rm -rf /usr/share/nginx/html
   mv /tmp/html /usr/share/nginx/
```

## 26. Quiz: Overriding NGINX Defaults

### QUIZ QUESTION
What configuration is optimal for an init script to fetch data from an S3 bucket?
* IAM permissions set via an IAM role

## 27. Exercise: Overriding NGINX Defaults

In this exercise, you will launch an EC2 instance with an IAM role and pull static website content from an S3 bucket to overwrite the default NGINX website.

### Exercise Requirements
### Prerequisites
* Download zip file for [Bootstrap SB2 Admin Theme Site](https://startbootstrap.com/theme/sb-admin-2)
* Upload the zip file to your <strong>S3</strong> bucket under a folder called <strong>web</strong> (do not extract it)

### EC2 Requirements
* <strong>AMI:</strong> Amazon Linux 2
* <strong>IP Address:</strong> Public
* <strong>Type:</strong> t2.micro
* <strong>IAM Role:</strong> web (created in the previous exercise)
* <strong>Security group:</strong> accessible from <strong>anywhere</strong> on <strong>port 80</strong>
* <strong>Init Script:</strong> see below

### Init Script
Copy the following script into the <strong>User data</strong> text box in the EC2 Instance Launch Wizard.

### Note: you must change the to your bucket name (with no spaces after the = sign)

```
   #!/bin/bash

   BUCKET_NAME=<s3-bucket-name-place-holder>
   yum update -y
   amazon-linux-extras install nginx1.12 -y
   service nginx start
   aws s3 cp s3://${BUCKET_NAME}/web/startbootstrap-sb-admin-2-gh-pages.zip /tmp/
   cd /tmp
   unzip start*
   mv startbootstrap-sb-admin-2-gh-pages html
   rm -rf /usr/share/nginx/html
   mv /tmp/html /usr/share/nginx/
```

### Goal
You should be able to see the SB Admin 2 web page with images displayed in the browser.

### Init Script Explanation
This is not necessary to understand in order to complete the exercise. But in case you are interested, here is what the init script does.

The init script installs Nginx web server.

Then it uses the [aws-cli s3 cp command](https://docs.aws.amazon.com/cli/latest/reference/s3/cp.html) to copy the <strong>Bootstrap Theme</strong> zip file from <strong>S3</strong> into the <strong>/tmp</strong> directory on the EC2 instance. Next, the init script extracts the file using the <strong>unzip</strong> command.

Finally, the init script overrides the contents of the <strong>/usr/share/nginx/html</strong> directory with the contents of the unzipped folder.

![](https://video.udacity-data.com/topher/2020/April/5e8e30dc_screen-shot-2020-04-08-at-13.15.14/screen-shot-2020-04-08-at-13.15.14.png)

## 28. Solution: Overriding NGINX Defaults Exercise

### Upload to S3
* 1. Navigate to the S3 console and select your bucket
* 2. Create a folder called ```web``` in your bucket
* 3. Upload the SB Admin 2 bootstrap theme zip file to the ```web``` folder

### Launching an EC2 instance using the EC2 Console
* 1. Navigate to the EC2 Instances Dashboard
* 2. Click on the <strong>Launch instance</strong> button
* 3. Choose the <strong>Amazon Linux 2 AMI (HVM), SSD Volume Type 64-bit</strong> image
* 4. Leave the default instance type as <strong>t2.micro</strong> and click <strong>Next: Configure instance details</strong>
* 5. Set the <strong>Auto-assign Public IP</strong> to <strong>enabled</strong>
* 6. Set the <strong>IAM role</strong> to be <strong>web</strong>
* 7. Copy the following script into the <strong>User data</strong> text box <strong>(Note: you must change the to your bucket name (with no spaces after the = sign))</strong>

```
#!/bin/bash

BUCKET_NAME=<s3-bucket-name-place-holder>
yum update -y
amazon-linux-extras install nginx1.12 -y
service nginx start
aws s3 cp s3://${BUCKET_NAME}/web/startbootstrap-sb-admin-2-gh-pages.zip /tmp/
cd /tmp
unzip start*
mv startbootstrap-sb-admin-2-gh-pages html
rm -rf /usr/share/nginx/html
mv /tmp/html /usr/share/nginx/
```
* 8. Click on the <strong>Review and Launch</strong> button and then click on the <strong>Launch</strong> button
* 9. Wait about 20-30 seconds for the instance to come up and for the script to finish running
* 10. Using a browser, visit the web page at the public IP address

![](https://video.udacity-data.com/topher/2020/April/5e8e30dc_screen-shot-2020-04-08-at-13.15.14/screen-shot-2020-04-08-at-13.15.14.png)

## 29. Edge Cases

### When Is EC2 Sub-Optimal?
EC2 resources (memory, CPU) are configured by instance types.

If a process is short-lived or does not need to be running constantly, and its footprint is much smaller than the EC2 instance resources. It might be better to use serverless functions rather than EC2, as a serverless approach will take fewer resources and is designed for short-lived processes.

### QUIZ QUESTION
Where EC2 is sub-optimal?
* When you have a short-lived jobs with minimal resource usage

## 30. Lesson Recap

In this lesson, you:

* Launched an EC2 instance
* Automatically installed NGINX on the server
* Connected EC2 with an S3 bucket via an IAM role
* Replaced the NGINX default webpage with content from an S3 bucket
* Opened connections to the EC2 instance from anywhere via a security group

In the next lesson, you will:

* Execute serverless computing via Lambda functions
* Connect Lambda Functions with the API Gateway
* Create an in-memory NoSQL database
* Test both the API Gateway and Lambda

![](https://video.udacity-data.com/topher/2020/June/5edc6f1b_course-outline/course-outline.png)

### Further Reading
### Documentation
* IAM Getting Started (https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html)
* IAM roles for EC2 (https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-roles-for-amazon-ec2.html)
* EC2 Getting Started (https://aws.amazon.com/ec2/getting-started/)
* EC2 best practices (https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-best-practices.html)
* Security Groups (https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html)

### Books
* Programming EC2 (https://www.amazon.com/Programming-Amazon-EC2-Survive-Success/dp/1449393683)

### Research
* Best Practices in Evaluating Elastic Load Balancing White Paper (https://aws.amazon.com/articles/best-practices-in-evaluating-elastic-load-balancing/)

### Blog Posts
* EC2 for beginners (https://towardsdatascience.com/aws-ec2-for-beginners-56df2e820d7f?gi=946a9446d8d5)
* AWS IAM Summary (https://enlear.academy/aws-iam-summary-5d97bb129ae1?gi=50f00c0ce6ff)
* EC2 T2 Insatnces (https://aws.amazon.com/ec2/instance-types/t2/)

### Advanced Topics
* AWS Nitro System - the system beyond standard virtualization (https://aws.amazon.com/ec2/nitro/)
* Auto Scaling (https://aws.amazon.com/autoscaling/)
* Elastic Load Balancing (https://aws.amazon.com/elasticloadbalancing/)

## 31. Glossary

* <strong>EC2:</strong> Elastic Compute Cloud, this is AWS's foremost compute service

* <strong>EC2 Instance:</strong> A virtual server running applications or software in AWS

* <strong>Elastic IP:</strong> A static IP allocated to your account that can be associated and disassociated from EC2 instances

* <strong>IAM Role:</strong> An IAM identity that has no long-term credentials and acts on behalf of the trusted user or service

* <strong>Init Script:</strong> An automation script that provisions and configures an instance on first boot

* <strong>NGINX:</strong> A web server for static and dynamic HTML pages

<strong>Security Group:</strong> A firewall ruleset to control traffic to and from AWS resources

________________________________________________________________________________________________________________________________________________________________________________

# LESSON 5 CLOUD DATABASES AND SERVERLESS ARCHITECTURE

## 1. Serverless Computing

Serverless computing is a managed compute resource that provides backend services without the need for you to manage any infrastructure.

* Focus on development, not infrastructure
* Reduce the need for DevOps expertise
* Cost-effective - pay only for fractions of a second
* Infinite scalability

## 2. Lesson Outline

### Course Outline
In previous lessons, you:

* Learned about cloud computing
* Launched a virtual machine on your local computer
* Created IAM users and policies
* Uploaded objects to an S3 bucket
* Launched EC2 instances
* Configured an IAM role
* Provisioned an EC2 instance via an init script

![](https://video.udacity-data.com/topher/2020/June/5ede9ed1_course-outline/course-outline.png)

### Lesson Outline
In this lesson, we will build a complete serverless solution that won't require service management from our side at all. A <strong>Lambda Function</strong> will serve as our backend. The Lambda Function will store data in an <strong>ElastiCache Redis</strong> database. We will connect the Lambda with a serverless frontend called <strong>API Gateway</strong>.

We will also learn how to test the Lambda Function from the console, and how to test the API gateway integration with a tool called <strong>Postman</strong>.

### Learning Objectives
In this lesson, you will:

* Create an ElastiCache Redis server
* Create a Lambda Function from the AWS Console
* Program a Lambda Function with code from a pre-existing zip file
* Test a Lambda Function from the console
* Create an API Gateway
* Connect to an API gateway from the Lambda as a trigger
* Trigger the Lambda Function from API Gateway, using a tool called Postman

## 3. Big Picture

Serverless is a managed, native cloud architecture that shifts operational responsibility of servers to the cloud. That allows you, the developer, to focus on building applications and services without even thinking about the servers and software needed to run your code.

Cost-efficiency is intertwined with serverless because you only pay for what you use, whereas even virtual servers cost money to run 24/7.

In this lesson, we will use a serverless frontend called <strong>API Gateway</strong> which will send the request to a <strong>Lambda Function</strong>, which will serve as our backend.

That Lambda will either set or get the user's name from a managed, in-memory database service. The Lambda will return the name back to the user via the API Gateway.

![](https://video.udacity-data.com/topher/2020/June/5edea096_serverless-demo-architecture/serverless-demo-architecture.png)

## 4. ElastiCache

SQL --> Structured Query Language.

### Relational Databases
Are built from tables with a unique identifier for each role.  That unique identifier is used in other tables to create relationships on query-related data together.

This is the reason SQL is known as a relational database.

Relational databases can become hard to manage and performance degrades over time as more and more storage is needed.

To solve these problems and provide faster scalable performance a new type of database emerged called NoSQL. 

### NoSQL Databases
Don't have tables.  Are more flexible, scale more easily and can handle more data and load.  
Most are key-value based, or document based.

Key-values associate a value with a key.  The value can be either text or a list of other values.  The relationship between two keys is defined by what their values have in common.

A document-based NoSQL database stores data in any format

### Redis --> Is a type of NoSQL database
Redis is key-value --> An AWS managed service called ElastiCache is used to ease the set up proccess.  

### ElastiCache
In memory key-value data store which makes it super fast.

SQL DATABASES --> manage data in a write/read to disk process.

ElastiCache --> All in memory which is much faster, and can handle very large loads easily.

ELASTICACHE: Fully managed service.  You don't need to perform any management tasks, hardware provisioning, software patching, set-up, configuration, and backups are all handled by AWS.

The access is configured using security groups and it is limited to the network where your computer is running.

Can grow up to 170 terabytes.

### ElastiCache
* Managed, in-memory NoSQL database
* For security, instances are deployed to a private subnet by default and lack a publicly reachable address
* Redis is an open-source data store, whereas ElastiCache is AWS's proprietary service the hosts Redis databases for AWS users
* Great choice for real-time applications such as gaming, chat, and video
* Easily scalable and replicable

![](https://raw.githubuserconte)nt.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/23.jpg)
![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/24.jpg)
![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/25.jpg)

## 5. Quiz: ElasticCache

### QUIZ QUESTION
What type of database does the ElastiCache for Redis managed service provide?
* In-memory NoSQL database

## 6. IAM Policies

Use the <strong>manager</strong> IAM user to complete the exercises in this lesson. You will need to supply the required permissions for the <strong>manager</strong> user.

Navigate to the [IAM console](https://console.aws.amazon.com/iam/home) and select the <strong>manager</strong> user.

Add the following AWS managed policies (permissions):

* <strong>AmazonElastiCacheFullAccess:</strong> This will allow the creation and deletion ElasticCache instances
* <strong>AWSLambdaFullAccess:</strong> This will allow the creation, update, and deletion of serverless (Lambda) functions
* <strong>AmazonAPIGatewayAdministrator:</strong> This will allow the manager to configure API Gateway to connect to our Lambda Function via HTTP

## 7. Exercise: ElastiCache For Redis

In this exercise, you will launch a Redis instance on ElastiCache. You will continue to use this instance in the next exercise.

### Instructions
* <strong>Single node</strong> with <strong>no replication</strong>
* <strong>t2.micro</strong> type
* <strong>us-east-1 N.Virginia</strong> region
* Setup on the <strong>default VPC</strong>
* No encryption either <strong>in transit</strong> (No Auth) or <strong>at-rest</strong>
* Name the node <strong>redis</strong>

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=xafrdiyuIAg&t=5s)

Before you start, you need to get the Virtual Private Cloud ID of the default VPC:

### Default VPC ID
* 1. Open the [VPC console](https://console.aws.amazon.com/vpc/home?region=us-east-1)
* 2. Note the default VPC ID

![](https://video.udacity-data.com/topher/2020/April/5e8fd6d7_screen-shot-2020-04-09-at-19.15.14/screen-shot-2020-04-09-at-19.15.14.png)

### Create the ElastiCache Redis Instance
* 1. Open the [ElastiCache console](https://console.aws.amazon.com/elasticache/home?region=us-east-1#)
* 2. Change the region on the top right to be <strong>us-east-1 N.Virginia</strong>
* 3. Click <strong>Redis</strong> on the sidebar menu, then click the <strong>Create</strong> button
* 4. Name the instance <strong>redis</strong>
* 5. Change the number of replicas to 0
* 6. Change the <strong>Node type</strong> to be <strong>t2.micro</strong>
* 7. Save
 
![](https://video.udacity-data.com/topher/2020/April/5e8fd539_screen-shot-2020-04-09-at-19.08.18/screen-shot-2020-04-09-at-19.08.18.png)

* 8. Under the Advanced Redis Settings, set the <strong>Name</strong> to be <strong>redis-subnet</strong>
* 9. Set the <strong>Description</strong> to <strong>Redis Subnet</strong>
* 10. Change the VPC ID to the default VPC ID that you noted previously
* 11. Select <strong>us-east-1a</strong> as the subnet

![](https://video.udacity-data.com/topher/2020/April/5e8fd8c7_screen-shot-2020-04-09-at-19.23.24/screen-shot-2020-04-09-at-19.23.24.png)

* 12. Scroll down to the <strong>Backup</strong> section and deselect <strong>Enable Automatic backups</strong>
* 13. Click on the <strong>Create</strong> button

Wait a few minutes for the instance to initialize. You can refresh the dashboard using the refresh arrows icon in the top-right corner of the dashboard.

![](https://video.udacity-data.com/topher/2020/April/5e8fd9f0_screen-shot-2020-04-09-at-19.28.47/screen-shot-2020-04-09-at-19.28.47.png)

## 9. Lambda Functions

Runs the code automatically, without the need to provision or manage servers.

Simply, write your code, upload it to Lambda and run.

Your code can run multiple times and in parallel.

Supports multiple languages and there is not need to install any software.

![](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/26.jpg)

Can have multiple triggers.

### Lambda Function
* Serverless fast solution to run code for a task
* Write code directly in the AWS console or upload a zip package with dependencies
* Supports multiple code languages
* Can be tested from the console

![](https://video.udacity-data.com/topher/2020/June/5edee29e_lambda-triggers/lambda-triggers.png)

## 10. Quiz: Lambda Functions

### QUIZ QUESTION
How do you add code with dependencies to Lambda?
* Create a zip of the code and dependancies and upload the zip to the Lambda

## 11. Exercise: Hello from Lambda
In this exercise, you will create a basic Lambda Function.

### Instructions
* Create a Lambda Function from scratch
* The Lambda Handler should be set to the default <strong>lambda_function.lambda_handler</strong>
* Manually trigger the Lambda via a test event and verify the message "Hello from Lambda"

## 12. Solution: Hello from Lambda Exercise

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=y2Z2DqZopRw&t=1s)

### Solution: Hello from Lambda
* 1. Navigate to the Lambda Console by searching for <strong>Lambda</strong> under <strong>Find Services</strong>

![](https://video.udacity-data.com/topher/2020/June/5edf09bd_screen-shot-2020-06-08-at-20.58.16/screen-shot-2020-06-08-at-20.58.16.png)

* 2. Click the <strong>Create function</strong> button and select <strong>Author from scratch</strong>
* 3. Name the function <strong>hello</strong>
* 4. Set the runtime to <strong>Python3.8</strong>
* 5. Click the <strong>Create Function</strong> button

![](https://video.udacity-data.com/topher/2020/June/5edf09ca_screen-shot-2020-06-08-at-20.58.48/screen-shot-2020-06-08-at-20.58.48.png)

* 6. Notice the <strong>handler</strong> field on the embedded code page. It's format is <strong>file-name.function-name</strong>. In our case, the file name is <strong>lambda_function.py</strong> and the code function name is <strong>lambda_handler</strong>, which is why the handler is pre-set to <strong>lambda_function.lambda_handler</strong>.

![](https://video.udacity-data.com/topher/2020/June/5edf09de_screen-shot-2020-06-08-at-20.59.12/screen-shot-2020-06-08-at-20.59.12.png)

* 7. Click on the <strong>Test</strong> button and configure a test event.
* 8. Name the event <strong>hellotest</strong> and save the event.

![](https://video.udacity-data.com/topher/2020/June/5edf09ec_screen-shot-2020-06-08-at-21.00.12/screen-shot-2020-06-08-at-21.00.12.png)

* 9. Click the <strong>Test</strong> button again while the <strong>hellotest</strong> event is pre-selected

![](https://video.udacity-data.com/topher/2020/June/5edf09fc_screen-shot-2020-06-08-at-21.00.29/screen-shot-2020-06-08-at-21.00.29.png)

* 10. Expand the <strong>Execution result</strong>
* 11. Verity the message: <strong>"Hello From Lambda!"</strong>

![](https://video.udacity-data.com/topher/2020/June/5edf0a07_screen-shot-2020-06-08-at-21.01.07/screen-shot-2020-06-08-at-21.01.07.png)


## 13. Exercise: Lambda Events

### Exercise: Lambda Events
* Modify the <strong>testhello</strong> event for the Lambda with the existing field:
```{"user": "Udacity"}```
* Modify the Lambda Function code to read the user out of the event field and display "Udacity".

## 14. Solution: Lambda Events Exercise

Please open the link in a new tab to watch the tutorial:

[![IMAGE ALT TEXT](https://raw.githubusercontent.com/ARBUCHELI/INTRO-TO-CLOUD-COMPUTING/master/images/19.jpg)](https://www.youtube.com/watch?v=Ta-z9Qf1wlM&t=1s)

### Solution: Lambda Events Exercise
* 1. From the ```hello``` Lambda Function, click on the <strong>hellotest</strong> dropdown menu and select <strong>Configure test events</strong>

![](https://video.udacity-data.com/topher/2020/June/5edf0df2_screen-shot-2020-06-08-at-21.12.25/screen-shot-2020-06-08-at-21.12.25.png)

* 2. Select <strong>Edit saved test events</strong> option (it should be pre-selected already)
* 3. Change <strong>key1</strong> to be <strong>"user"</strong>
* 4. Change the value for <strong>"user"</strong> to be <strong>"Udacity"</strong>
* 5. Click Save Event

![](https://video.udacity-data.com/topher/2020/June/5edf0e03_screen-shot-2020-06-08-at-21.13.52/screen-shot-2020-06-08-at-21.13.52.png)

* 6. Edit the code in the editor and set the <strong>body</strong> on <strong>line 7</strong> to be:

```json.dumps(event["user"])```

* 7. Click Save.

![](https://video.udacity-data.com/topher/2020/June/5edf0e15_screen-shot-2020-06-08-at-21.14.33/screen-shot-2020-06-08-at-21.14.33.png)

* 8. Click the <strong>Test</strong> button.
* 9. Expand the results.
* 10. Verify message: <strong>Udacity</strong>

![](https://video.udacity-data.com/topher/2020/June/5edf0e26_screen-shot-2020-06-08-at-21.15.04/screen-shot-2020-06-08-at-21.15.04.png)































































