
This CloudFormation template establishes a fundamental three-tier architecture within an AWS environment. The architecture comprises three layers: Presentation (Web Server), Application, and Data. Each layer is represented by EC2 instances with associated security groups.

#### Presentation Layer (Web Server):
- **WebServerSecurityGroup:** Defines a security group allowing HTTP traffic (port 80) from any source.
- **WebServerInstance:** Launches an EC2 instance of type t2.micro, using a specified AMI (Amazon Machine Image), and associates it with the WebServerSecurityGroup.

#### Application Layer:
- **AppServerSecurityGroup:** Establishes a security group permitting internal traffic on port 8080 within the specified CIDR range.
- **AppServerInstance:** Deploys an EC2 instance (t2.micro) with a designated AMI, linked to the AppServerSecurityGroup.

#### Data Layer (Database):
- **DatabaseSecurityGroup:** Specifies a security group enabling internal traffic on port 3306 for database communication within the defined CIDR range.
- **DatabaseInstance:** Creates an EC2 instance (t2.micro) using a specified AMI and associates it with the DatabaseSecurityGroup.

This architecture provides a foundation for hosting scalable web applications with distinct layers for presentation, application logic, and data storage. It's important to replace the placeholder AMI IDs with relevant IDs for each layer, and adjust CIDR ranges according to your VPC configuration.

### How to Use:
1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/yourusername/aws-repo.git
   ```

2. Navigate to the `cloudformation` directory.
   ```bash
   cd aws-repo/cloudformation
   ```

3. Deploy the CloudFormation template using the AWS Management Console, AWS CLI, or AWS SDKs.

Feel free to explore and modify the template based on your specific requirements or use it as a starting point for more complex architectures. If you have any questions or suggestions, please open an issue or contribute to the repository.