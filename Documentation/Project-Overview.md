# Project Overview: Highly Available WordPress Deployment  

## Objective
The goal of this project is to deploy a WordPress site on AWS with high availability, fault tolerance, and scalability.  

## Key AWS Services Used
- **EC2 (Elastic Compute Cloud)**: Hosts the WordPress application.
- **RDS (Relational Database Service)**: Manages the MySQL database.
- **EFS (Elastic File System)**: Provides shared file storage for WordPress instances.
- **ELB (Elastic Load Balancer)**: Distributes incoming traffic across EC2 instances.
- **S3 (Simple Storage Service)**: Stores WordPress media files.
- **Auto Scaling Group (ASG)**: Ensures sufficient instances are always available.

## High-Level Workflow
1. Users access the WordPress site via a domain.
2. Traffic is routed through the ELB, which balances the load across EC2 instances in multiple AZs.
3. The EC2 instances use RDS for database queries and EFS for shared storage.
4. Media files are stored and served from S3.

This setup ensures high availability and fault tolerance, making it suitable for production-grade applications.

