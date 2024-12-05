# Troubleshooting Guide  

## Common Issues and Solutions  

### 1. EC2 Instances Not Connecting to RDS
- **Issue**: Cannot connect to the RDS database.
- **Solution**: Ensure security groups allow EC2 access to RDS on port 3306.

### 2. Media Files Not Uploading to S3
- **Issue**: Media files are not being offloaded to S3.
- **Solution**: Install necessary PHP extensions like cURL, XMLWriter, and SimpleXML.

### 3. EFS Not Mounted on EC2
- **Issue**: EFS volume is not accessible.
- **Solution**: Verify EFS mount point and ensure `nfs-utils` is installed and ensure that security groups allow EC2 access to EFS on port 2049.

### 4. Load Balancer Not Routing Traffic
- **Issue**: Users cannot access the site through the ELB.
- **Solution**: Check ELB listener configuration and health checks.

