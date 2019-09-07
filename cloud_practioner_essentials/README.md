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



