# Mini Project: Understanding Environment Variables & Infrastructure Environments

## Project Overview
This project explores the difference between **Infrastructure Environments** (e.g., development, testing, production) and **Environment Variables** (key-value pairs that configure applications).  
The goal is to demonstrate how shell scripting can use environment variables to manage different infrastructure environments effectively.

## Key Learning
- **Environment Variables**: How to set, export, and use them in scripts.  
- **Infrastructure Environments**: How different environments (dev, test, prod) are structured and why they matter.  
- **Conditional Logic in Scripts**: Running different commands based on the environment selected.  
- **Automation Benefits**: Reducing manual setup, improving consistency, and increasing flexibility.  

## Script Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/slarry07/env-variables-project.git
   cd env-variables-project

Make the script executable:
chmod +x aws_cloud_manager.sh

Run for different environments:
./aws_cloud_manager.sh dev
./aws_cloud_manager.sh test
./aws_cloud_manager.sh prod

Project Structure
.
├── aws_cloud_manager.sh   # Main script
├── .env.dev               # Dev environment variables
├── .env.test              # Test environment variables
├── .env.prod              # Prod environment variables
└── README.md              # Documentation


