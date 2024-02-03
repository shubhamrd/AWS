# AWS CloudFormation Examples

Welcome to the AWS CloudFormation directory within the AWS Training Repository. This section contains a collection of CloudFormation templates to help you automate the deployment of AWS resources. Each template is designed to showcase specific use cases, services, or configurations.

## List of CloudFormation Templates

1. [**Three Tier Architecture**](three-tier)
   - A CloudFormation template defining a basic three-tier architecture with EC2 instances for presentation, application, and data layers.

2. [**S3 Bucket with Public Access**](s3-public-bucket.yaml)
   - Deploy an S3 bucket configured for public access. Useful for hosting static websites or publicly accessible files.

3. [**VPC with Public and Private Subnets**](vpc-public-private.yaml)
   - Create a VPC with public and private subnets, including NAT gateways for private subnet internet access.

4. [**Auto Scaling Group with Load Balancer**](asg-lb.yaml)
   - Demonstrates the use of Auto Scaling Groups with an associated Application Load Balancer for scalable and resilient applications.

5. [**RDS Database Instance**](rds-instance.yaml)
   - Set up a Relational Database Service (RDS) instance with customizable parameters. Ideal for deploying database solutions.

## Getting Started

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/aws-repo.git
