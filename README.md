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



















