[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/README.md)   [![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/README_PT-BR.md)

# Cloud: Final Project - PB
AWS - Cloud Practitioner - PB Aws - IF Fluminense - IFMT - UTFPR - UNAMA  | Scholarship Program - DevSecOps

#### Team Members:
- [Bruno Garcia Nazareth](https://github.com/brunoshure)
- [Nicolas Meirelles Grisostolo](https://github.com/zSalocin)
- [Raphael Antunes Marinho de Souza](https://github.com/RaphaelAntunesMarinhoDeSouza)

### Case:
"Fast Engineering S/A" is seeking a solution from the third-party company "AMAZING IT SOLUTIONS". Fast Engineering's eCommerce is experiencing significant growth, and the current solution is no longer able to handle the high demand for access and purchases it is facing. Since the beginning of the year, accesses and purchases have been increasing by 20% every month.

**Current Architecture**
* 01 server for MySQL Database;
* 01 server for the application using REACT;
* 01 web server that stores static assets such as photos and links.

**Order Requirements**
- Scope.
- Architecture of the New Solution.
- Costs.
- Delivery Deadline.
- Macro Shedule of Deliveries.

For the construction of the architecture for our company's future website, it is necessary to follow the best DevOps practices.

**New Architecture Requirements**
- Kubernetes Environment.
- PaaS Database.
- MultiAZ.
- Data backup security.
- Data persistence.
- Load balancing with health check.
- Security (grant only necessary/minimum access).

Objective: Develop the proposal and architecture of what the team proposes to deliver.

___

## AWS Migration Project - Fast Engineering S/A

## Introduction

This repository contains the documentation and scope of the AWS migration project for an e-commerce platform. The project aims to increase scalability and reduce operational costs.

## Client's Motivation

The motivation behind this migration is the need to meet the growing demand for access and purchases that Fast Engineering S/A is facing.

## Project Scope

### Assessment of Current Infrastructure.

![Current_Architecture](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Arquitetura_Atual.png)

### Proposed Solution Architecture:

The proposed architecture follows best practices and aligns with the AWS Well-Architected Framework.

  **AWS Well-Architected Framework Pillars**
      
![Current_Architecture](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Pilares.png)
  
  **Data Migration**
  
 The team is implementing a crucial database migration to AWS RDS, prioritizing efficiency and operational continuity. The AWS Database Migration Service (DMS) will be used to ensure a smooth transition, replicating data continuously while maintaining its integrity. This strategy aims to minimize any impact on daily operations while leveraging the scalability and security benefits offered by AWS. The team is committed to ensuring that this migration is a smooth and successful transition.

  **Services Used**
  
- **Amazon CloudFront**
  Amazon CloudFront is a Content Delivery Network (CDN) service offered by Amazon Web Services (AWS). Its main function is to accelerate the delivery of static and dynamic content, such as web pages, images, videos, scripts, and other multimedia files, to end-users with low latency and high availability.
  
- **AWS Web Application Firewall (WAF)**
  - AWS Web Application Firewall is a firewall service designed to protect web applications against common attacks, providing advanced protection against threats and ensuring the security of web applications.

- **AWS Shield**
  - AWS Shield is a security service that protects AWS applications and resources against Distributed Denial of Service (DDoS) attacks, providing defense against high-level DDoS attacks to maintain resource availability.

- **Amazon Route 53**
  - Amazon Route 53 is a DNS service that allows you to register and manage domains, with traffic routing to AWS resources such as ELB and CloudFront. It facilitates efficient traffic routing and ensures high availability by directing access to AWS instances and services.

- **Amazon Simple Storage Service (S3)**
  - Amazon S3 uses Buckets to store and distribute static content, including images, videos, and files, integrating with CloudFront for efficient delivery. It offers secure and scalable storage for images, videos, and files.

- **Amazon EKS**
  - Elastic Kubernetes Service acts as the foundation of the architecture, offering container orchestration through Kubernetes. It provides scalable container orchestration, allowing dynamic expansion and high availability of the application.

- **Amazon Virtual Private Cloud (VPC)**
  - Virtual Private Cloud isolates the cloud infrastructure and provides granular control over the network by creating a virtual private network. It establishes a VPC network, improving traffic control and infrastructure security.

- **Amazon RDS** 
  -Amazon RDS (Relational Database Service) is a relational database service offered by Amazon Web Services (AWS). It is designed to simplify the administration, operation, and scalability of relational databases, allowing developers to focus on their applications without worrying about managing the underlying database.

- **Elastic Load Balancing**
  - Elastic Load Balancing is a service that distributes traffic among multiple instances or resources to ensure high availability and scalability of applications.

- **Amazon CloudWatch**
  - Amazon CloudWatch is a monitoring and observation service that provides insights into the performance of AWS resources and applications.

- **AWS Database Migration Service**
  - AWS Database Migration Service facilitates the migration of databases to AWS securely and easily.

- **AWS CodeBuild**
  - AWS CodeBuild is a fully managed build service that compiles source code, runs tests, and creates artifacts.

- **AWS CodePipeline**
  - AWS CodePipeline is a continuous delivery service that automates the building, testing, and deployment of applications.

- **AWS CodeDeploy**
  - AWS CodeDeploy is an automated deployment service that makes it easier to deploy applications on AWS.

- **Amazon EC2**
  - Amazon EC2 provides on-demand virtual instances with customizable configurations for a wide range of workloads. It offers on-demand scalability, allowing for quick adaptation to computing needs without upfront investments in physical hardware.

- **AWS Backup**
  - AWS Backup is a fully managed backup service that helps simplify data protection and resource recovery in AWS.

- **CloudFormation**
  - AWS CloudFormation is a service that allows you to create and manage AWS resources through infrastructure-as-code templates.
 
  **New Architecture**
  
![PROJECT_ARCHITECTURE](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Arquitetura.jpeg)

### Values
AWS Calculator:

Access the [AWS pricing calculator](https://calculator.aws/#/)

[New Architecture Estimate](https://calculator.aws/#/estimate?id=f0691a4bdf6209114ce6b6391e274d6b089bec07)

**Costs**

|        Item           |                 Description                |       Price       |
|-----------------------|--------------------------------------------|-------------------|
| Migration to AWS      | On-premise data migration to AWS           | $496,40           |
| AWS Infrastructure    | Cost of AWS services infrastructure        | $4.859,38/monthly |
| Team Cost             | Technical support and maintenance          | $3.457,76/monthly |

### Delivery Deadline

+ Architecture implementation: **28 business days**.

Team of 3 people:
  - Working 8 hours a day
  - Over the course of 28 business days
  - Total of 672 hours for delivery.

### Macro Schedule of Deliveries

![Cronograma](https://github.com/zSalocin/PB_Compass_Projeto_Final_Arquitetura/blob/main/Assets/Cronograma.jpeg)