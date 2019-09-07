# AWS Cloud Practitioner Essentials (Second Edition)

> In this digital, self-paced course, you’ll gain an overall understanding of AWS Cloud, independent of specific technical roles. It provides a detailed overview of cloud concepts, AWS services, security, architecture, pricing, and support. This course also helps you prepare for the AWS Certified Cloud Practitioner exam. - [Source](https://aws.amazon.com/training/course-descriptions/cloud-practitioner-essentials/)

## Course Introduction
* Introductory video to the AWS Cloud Practitioner Essentials course ([video](https://www.aws.training/Details/eLearning?id=29804))
    + This course will give an overview of AWS
    + Guide to AWS services
    + Overview of cloud architecture
    + I should be able to...
        + Define what the AWS cloud is and its global infrastructure;
        + Describe basic AWS Cloud architectural principles;
        + Understand the AWS Cloud value proposition;
        + Talk about key AWS services and their basic use cases;
        + Define the billing, account management, and pricing models;
        + Identify sources of documentation or technical assistance; and
        + Describe the characteristics of deploying and operating in the AWS Cloud.
    + Course should take about 6 hours to complete.

## Introduction to the AWS Cloud

* This module provides an introduction to the AWS Cloud and the methods available to interact with various AWS services.
    + Goal: define what the AWS cloud is and its global infrastructure.

* Cloud computing definition
    + On-demand delivery of IT resources and applications via the Internet.
    + History
        + Prior to cloud computing, we had to build data centers by guessing what our maximum peaks might be.
        + If the design didn't meet our maximum needs, our customers would suffer.
        + If the design over estimated maximum need, we ended up paying for resources that we didn't really need.
    + With cloud computing, we can scale the resources up or down based on our real-time needs. In short, we pay for what we actually use without having to plan for the worst.

+ AWS allows us to access servers, databases, storage, and higher level application components.
    + Change management, testing, reliability, and capacity planning is more agile and efficient.

* AWS helps reduce risk
    + Financially: an IT investment can be monitored to determine whether to scale up or down at a moment's notice.
    + Security: test often, patch quickly, and respond to incidents at lightning speed.
    + Quickly and elastically to market conditions.

+ AWS helps with scaling
    + Scalability: resize your resources.
    + Customers can grow or shrink their resources based on strategy (i.e. more resources during the holidays; less during the slower months)

* AWS helps with agility
    + Increase speed;
    + Decrease cost of experimentation; and
    + Cultivating culture of innovation.

* AWS easy to access resources
    + Start up or shut down services;
    + Testing is easier with development and production purposes in mind.

* Elasticity: scale computing power as the workload grows, and instantly shut down resources when demand drops.

* AWS allows you to deploy your systems around the world. Thanks to efficiencies of scale, AWS helps make cloud computing affordable.

* Reliability is key to mitigate disruptions. Architecture and systems must be in place to detect failures to allow for quick patches.

* AWS regions consist of availability zones. Each availability zone is isolated into different connectivity housed facilities. This is fault tolerant in the event any one of the facilities fail.

* Security of customers' data is now done constantly due to the monitoring capabilities of AWS.
    + Highly secure data centers;
    + Securely staffed 24/7;
    + Limit of access to the secure data center; and
    + Minimize risk of disruption and system failure.

+ AWS is trusted by the largest enterprises across the world.

## Introduction to AWS Interfaces

* This module teaches us about the convenient options for accessing and using AWS resources.
    + AWS Management Control
        + Easy-to-use graphical interface that supports majority of Amazon Web Services
    + Command Line Interface (CLI)
        + Access to services via discrete commands
    + Software Development Kits (SDKs)
        + Incorporate the connectivity and functionality of the wide range of AWS Cloud services into your code with support for popular programming languages

* Usability benefits
    + AWS Management Control
        + Navigation;
        + Usability; and
        + Convenient mobile app.
    + Command Line Interface (CLI)
        + Programming language agnostic; and
        + Flexible to create scripts.
        + Open source tool built for interacting with AWS services.
            + Environments:
                + Linux: Linux, Unix, or macOS;
                + Windows: PowerShell or Windows Command Processor; and
                + Remotely: Run commands on Amazon EC2 instances, SSH, or with Amazon EC2 systems manager.
    + Software Development Kits (SDKs)
        + Ability to use AWS in existing applications; and
        + Flexibility to create applications.
        + Infrastructure as code is a new concept:
             + Use of AWS specific API for a number of popular languages (i.e. Python, C++, Ruby, Go, .NET, etc.)

* You can use all three!
     + You may create an AWS EC2 instance using an SDK, describe it using the AWS CLI, and shut it down with just a few clicks from Management Console.
     + However....
         + If you make changes to a feature using the CLI, it might not be readily viewable from the console when it initially launches.

## Core Services

This module will provide high level information regarding a variety of core services provided by AWS platform, along with their common use cases.

### Elastic Compute Cloud (EC2)

* What is EC2?
     + It stands for Elastic Compute Cloud (EC2)
     + The following are a few examples of its use:
         + Application server;
         + Web server;
         + Database server;
         + Game server;
         + Mail server;
         + Media server;
         + Catalog server;
         + File server;
         + Computing server;
         + Proxy server; and
         + etc.
     + Cloud refers to the fact that these are cloud hosted resources
     + Elastic refers to the fact that, if properly configured, you can increase or decrease the amount of servers required by an application automatically according to the current demands of the application.

* Formally known as Amazon EC2 Instances
    + Pay-as-you-go: you only pay for running instances and the time they run.
    + Broad selection of Hardware/Software
    + Global hosting
    + For more info, see: https://aws.amazon.com/ec2/

+ Product Demonstration
    + Login to AWS Console;
    + Choose a region where we are going to host our instance;
         + Note: teacher selected Oregon because they said it was close by. Taking that to mean you should select a region nearest your customers.
    + Launch EC2 wizard;
    + Select Amazon Machine Image (AMI) (Software);
        + An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch your instance. You can select an AMI provided by AWS, our user community, or the AWS Marketplace; or you can select one of your own AMIs.
        + The tutorial selected "Amazon Linux AMI (2017)"
    + Select instance type (Hardware);
        + Amazon EC2 provides a wide selection of instance types optimized to fit different use cases. Instances are virtual servers that can run applications. They have varying combinations of CPU, memory, storage, and networking capacity, and give you the flexibility to choose the appropriate mix of resources for your applications.
        + The tutorial selected the "t2.micro" instance type
    + Configure network;
        + Configure the instance to suit your requirements. You can launch multiple instances from the same AMI, request Spot instances to take advantage of the lower pricing, assign an access management role to the instance, etc.
        + The tutorial selected the default "Network", "Subnet", and "Auto-assign Public IP" which gives us a [DHCP](https://kb.iu.edu/d/adov) address
    + Configure storage;
        + Your instance will be launched with the following storage device settings. You can attach additional EBS volumes and instance store volumes to your instance, or edit the settings of the root volume. You can also attach additional EBS volumes after launching an instance, but not instance store volumes. For more information, see here: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Storage.html.
    + Configure tags;
        + A tag consists of a case-sensitive key-value pair. For example, you could define a tag with `key = Name` and `value = Webserver`. A copy of a tag can be applied to volumes, instances, or both. Tags will be applied to all instances and volumes. For more information, see here: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Tags.html.
        + By default, an EC2 instance is given a rather cryptic identifier. This is known as the 'Instance ID'.
        + Tags allow us to give it a friendlier name. This is known as the EC2 'Name'.
    + Configure security group; and
        + A security group is a set of firewall rules that control the traffic for your instance. On this page, you can add rules to allow specific traffic to reach your instance. For example, if you want to set up a web server and allow Internet traffic to reach your instance, add rules that allow unrestricted access to the HTTP and HTTPS ports. You can create a new security group or select from an existing one below. For more information, see here: https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/security-group-rules-reference.html.
        + The tutorial created a new security group. Named it `ssh-http`. And added two rules: one type for SSH and HTTP.
    + Configure key pairs that allow us to connect to the instance after we launch it;
        + A key pair consists of a **public key** that AWS stores, and a **private key** that you store. Together, they allow you to connect to your instance securely.
        + For Windows AMIs, the private key is required to obtain the password used to log into your instance.
        + For Linux AMIs, the private key file allows you to securely SSH into your instance.
        + Name the key-pair name and download the `<key-pair-name>.pem` file locally.
        + Note: at this point, the tutorial does nothing with the `<key-pair-name>.pem` file.
    + Ah: the tutorial is using Windows. They launch PuTTy (`putty.exe`).
        + They copy the Public DNS (IPv4) name into the IP Address text box. It looks like `ec2-35-160-128-192.us-west-2.compute.amazonaws.com`. They paste that url after typing `ec2-user@<public-dns-url>`.
        + They leave the port as `22`.
        + They leave the connection type as `SSH`
        + Error! It doesn't open because we haven't configured the private key yet.
        + Relaunches `PuTTy` and recopies the same DNS url into the "Host Name" text box: `ec2-user@<public-dns-url>`.
        + From the left-hand side, they click on `SSH` -> `Auth`. They then browse for the private `<key-pair-name.pem` file (i.e. the file that stores the private key)
        + At this point, the teacher mentions that Windows requires the conversion of a `.pem` file to a `.ppk` file. They launch `puttygen.exe` and convert the `.pem` file to a `.ppk` file.
        + After the conversion, they went back to `putty.exe`, identified the location of the newly created `<key-pair-name.ppk` file, and were able to successfully launch their EC2 instance.




