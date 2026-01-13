# AWS Resource Listing Shell Script

A Bash script to list AWS resources from a given AWS account using the AWS CLI. This script helps quickly fetch details of commonly used AWS services in a specified region, making it useful for learning, auditing, and automation tasks.

---

## 📌 Features

* Lists resources across multiple AWS services
* Uses AWS CLI commands internally
* Simple and easy-to-use command-line interface
* Helpful for beginners learning **Shell Scripting + AWS**
* Reduces manual effort in checking AWS resources

---

## 🛠 Supported AWS Services

The script currently supports listing resources for the following services:

1. EC2
2. S3
3. RDS
4. DynamoDB
5. Lambda
6. EBS
7. CloudFront
8. CloudWatch
9. SNS
10. SQS
11. Route53
12. VPC
13. CloudFormation
14. IAM

---

## 📂 Prerequisites

Before running the script, ensure the following:

* **AWS CLI** is installed
* **AWS CLI** is configured with valid credentials (`aws configure`)
* Bash shell environment (Linux / macOS)
* Proper IAM permissions to list AWS resources

---

## 🚀 Usage

```bash
./aws_resource_list.sh <aws_region> <aws_service>
```

### Example

```bash
./aws_resource_list.sh us-east-1 ec2
```

This command will list all EC2 instances in the `us-east-1` region.

---

## 🔎 How It Works

1. Validates the number of input arguments
2. Checks if AWS CLI is installed
3. Verifies AWS CLI configuration
4. Uses a `case` statement to execute service-specific AWS CLI commands
5. Outputs the resource details in JSON format

---

## ⚠️ Error Handling

* Displays usage instructions if incorrect arguments are passed
* Exits if AWS CLI is not installed
* Exits if AWS CLI is not configured
* Handles invalid service names gracefully

---

## 📈 Future Enhancements

* Add support for more AWS services
* Pretty-print output using `jq`
* Menu-driven interface
* Support for AWS profiles
* Export output to files (JSON / CSV)

---

⭐ If you find this script helpful, feel free to star the repository and share feedback!
