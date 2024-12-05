# Deployment Steps  

Follow these steps to replicate the project:  

## 1. Setup VPC and Subnets
- Create a VPC and define subnets for multiple AZs.

## 2. Deploy RDS
- Launch a Multi-AZ MySQL RDS instance.
- Configure the database with WordPress tables.

## 3. Configure EFS
- Set up an EFS volume.
- Mount EFS on EC2 instance.

## 4. Create EC2 Instances with ASG
- Create an AMI with WordPress pre-installed and EFS mounted.
- Launch EC2 instances via an Auto Scaling Group.

## 5. Setup S3
- Create an S3 bucket for WordPress media files.
- Use the WP Offload Media plugin to configure S3 integration.

## 6. Configure ELB
- Create an Application Load Balancer (ALB).
- Link it with the ASG for traffic distribution.

## 7. Finalize Domain Setup
- Map the domain to the load balancer (using Route 53 or another DNS provider).

