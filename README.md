
# AWS EC2 Cloud Security Lab

## Project Overview
This hands-on project demonstrates secure deployment and administration of an Amazon EC2 instance using AWS cloud security best practices.

## AWS Services
- Amazon EC2
- Amazon VPC
- EC2 Security Groups
- Amazon Machine Images (AMI)

## Security Implementations

### 1. EC2 Deployment
- Launched an Amazon Linux 2023 EC2 instance.
- Selected an appropriate instance type.
- Configured instance networking.

### 2. SSH Key-Based Authentication
- Generated an EC2 key pair.
- Used a private key for SSH authentication.
- Restricted private key file permissions.

### 3. Security Group Configuration
- Allowed inbound SSH traffic on TCP port 22.
- Restricted SSH access to my public IP address.
- Avoided unrestricted SSH access from 0.0.0.0/0.

### 4. Secure Remote Access
Connected to the instance using:

```bash
chmod 400 key.pem
ssh -i key.pem ec2-user@<EC2-PUBLIC-IP>
```

### 5. Resource Lifecycle
- Studied EC2 running, stopped, and terminated states.
- Terminated the lab instance after testing.

## Security Concepts Learned
- Shared Responsibility Model
- Network Access Control
- SSH Authentication
- Least Privilege Network Access
- Cloud Attack Surface Reduction
- EC2 Security Best Practices

## Key Takeaway
Cloud security starts with securely configuring resources, restricting unnecessary access, and managing infrastructure throughout its lifecycle.
