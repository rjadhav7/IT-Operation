I'll help you set up a Terraform workflow to deploy EC2 resources with an Azure DevOps pipeline. Let me create a comprehensive solution for you.Now let me create a setup guide for you:Perfect! I've created a complete solution for deploying EC2 resources using Terraform with an Azure DevOps pipeline. Here's what I've provided:

## 📦 What's Included:

1. **Terraform EC2 Configuration** - Complete infrastructure code including:
   - EC2 instance with security group
   - Optional Elastic IP
   - Encrypted root volume
   - S3 backend for state management

2. **Variables & Outputs** - Flexible configuration with:
   - Configurable instance type, AMI, networking
   - Outputs for instance IDs, IPs, and security groups

3. **User Data Script** - Bootstrap script that installs:
   - Docker
   - Apache web server
   - Basic utilities

4. **Azure DevOps Pipeline** - Multi-stage pipeline with:
   - **Validate**: Syntax and format checking
   - **Plan**: Generate and review changes
   - **Apply**: Deploy with approval gate (production environment)
   - **Destroy**: Manual destruction stage (disabled by default)

5. **Comprehensive Setup Guide** - Step-by-step instructions covering everything

## 🚀 Key Features:

- **State Management**: Remote state in S3 with DynamoDB locking
- **Approval Gates**: Manual approval required before applying to production
- **Branch Strategy**: Full deployment on `main`, validation only on other branches
- **Security**: IAM-based authentication, encrypted volumes, security groups
- **Reusability**: Parameterized configuration using variables

## 📋 Quick Start:

1. Set up AWS resources (S3 bucket, DynamoDB table, IAM user)
2. Configure Azure DevOps (install Terraform extension, create service connection)
3. Push code to your Azure Repos
4. Create and run the pipeline

