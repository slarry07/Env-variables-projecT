# AWS Cloud Manager Script

## Overview
This project demonstrates how to use **environment variables** and **shell scripting** to manage different infrastructure environments (dev, test, prod) on AWS.  
The script provisions EC2 instances with different configurations depending on the environment.

## Features
- Environment-based logic using shell `case` statements  
- AWS CLI integration to launch EC2 instances  
- Clear separation of `dev`, `test`, and `prod` settings  
- Extensible for real-world deployments  

## Usage
1. Configure AWS CLI with valid credentials:
   ```bash
   aws configure
Make the script executable:
chmod +x aws_cloud_manager.sh

Run for a specific environment:
./aws_cloud_manager.sh dev
./aws_cloud_manager.sh test
./aws_cloud_manager.sh prod

Example Output
Launching dev environment EC2 instance...
{
    "Instances": [
        {
            "InstanceId": "i-0abcd1234efgh5678",
            "State": { "Name": "pending" },
            "InstanceType": "t2.micro",
            "Tags": [{ "Key": "Environment", "Value": "dev" }]
        }
    ]
}

Project Structure

.
├── aws_cloud_manager.sh   # Main script
└── README.md              # Documentation


