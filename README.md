# AWS Resource Lister

## Overview

This repository contains a Bash script designed to help users quickly list AWS resources from various services within a specified AWS region. It is ideal for learners, DevOps engineers, or cloud administrators who want to audit or explore AWS environments using the AWS CLI.

## Features

* Supports listing resources from multiple AWS services
* Simple command-line usage
* Validates input parameters and AWS CLI configuration
* Lightweight and easy to customize

## Supported AWS Services

The script currently supports the following services:

* EC2
* RDS
* S3
* CloudFront
* VPC
* IAM
* Route53
* CloudWatch
* CloudFormation
* Lambda
* SNS
* SQS
* DynamoDB
* EBS

## Prerequisites

To use this script, ensure the following requirements are met:

* AWS CLI is installed on your system
* AWS credentials are configured using `aws configure`
* Appropriate IAM permissions are granted to your AWS user
* Bash shell environment (Linux, WSL, or similar)

## Usage

### Step 1: Make the script executable

```bash
chmod +x aws_resource_list.sh
```

### Step 2: Run the script

```bash
./aws_resource_list.sh <aws_region> <aws_service>
```

### Example

```bash
./aws_resource_list.sh us-east-1 ec2
```

This command lists EC2 instances in the `us-east-1` region.

## Error Handling

* If parameters are missing, the script will show usage instructions.
* If the AWS CLI is not installed or not configured, the script will prompt you accordingly.
* If the specified IAM user lacks necessary permissions, AWS will return an authorization error.

## File Structure

```
aws-resource-lister/
├── aws_resource_list.sh   # Main script
├── README.md              # Project documentation
```

## Author

**Deepak B**

## Version

**v0.0.1** – Initial release

## License

This project is open-source and available for educational and personal use. Licensing terms can be added based on future needs.

## Contributions

Feedback and contributions are welcome. If you'd like to enhance this script or add support for more services, feel free to fork the repository and open a pull request.

---

For any questions or support, feel free to reach out via GitHub issues.
