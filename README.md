# AWS Cost Spike Alert System Using S3 and Lambda with Email Notifications

## 📌 Project Overview

Built a serverless AWS Cost Spike Alert System using Amazon S3, AWS Lambda, Python, and Amazon SNS.

The project uses a sample AWS cost and usage Excel file (`AWS_Cost_and_Usage_Practice.xlsx`) uploaded to an Amazon S3 bucket. Whenever a new file is uploaded, an S3 event notification automatically triggers an AWS Lambda function.

The Lambda function retrieves and processes the Excel data using Pandas and OpenPyXL, checks the cost against a predefined threshold, and identifies unexpected cost increases. If a cost spike is detected, Amazon SNS sends an automated email notification.

This project demonstrates event-driven automation, serverless computing, Python-based data processing, and cloud cost monitoring.

## 🏗️ AWS Architecture Diagram

The following diagram illustrates the workflow of the AWS Cost Spike Alert System.

![AWS Cost Spike Alert System](./AWS%20Cost%20Spike%20Alert%20System.png)

## 🛠️ AWS Services and Technologies Used

 Technology                           Purpose 

 Amazon S3                 Stores AWS cost and usage Excel data 
 AWS Lambda                Executes serverless Python code 
 Amazon SNS                Sends automated email notifications 
 AWS IAM                   Manages permissions between AWS services 
 Amazon CloudWatch         Monitors Lambda execution logs 
 Python                    Automation and data processing 
 Pandas                    Reads and analyzes Excel data 
 OpenPyXL                  Reads Excel (.xlsx) files 

## ⚙️ Project Workflow

1. Download the sample AWS cost and usage Excel file.
2. Upload the Excel file to an Amazon S3 bucket.
3. Configure an S3 event notification to trigger AWS Lambda.
4. Lambda retrieves the uploaded Excel file from S3.
5. Pandas and OpenPyXL process and analyze the cost data.
6. The processed cost is compared against a predefined threshold.
7. If a cost spike is detected, Amazon SNS publishes an alert.
8. An email notification is delivered to the subscribed email address.

## 📂 Project Structure

```text
AWS-Cost-Spike-Alert-System/
│
├── lambda_handler.py
├── AWS_Cost_and_Usage_Practice.xlsx
├── AWS Cost Spike Alert System.png
└── README.md
```


### File Description

- lambda_handler.py: Python Lambda function for processing Excel cost data, detecting cost spikes, and triggering SNS notifications.
- AWS_Cost_and_Usage_Practice.xlsx: Sample AWS cost and usage data used for testing.
- AWS Cost Spike Alert System.png: AWS architecture diagram.
- README.md: Project documentation.



## 🎯 Key Learnings

- Implemented event-driven architecture using Amazon S3 and AWS Lambda.
- Integrated S3 event notifications with Lambda.
- Processed Excel files using Python, Pandas, and OpenPyXL.
- Configured Amazon SNS for automated email notifications.
- Worked with AWS IAM roles and permissions.
- Monitored serverless application execution using CloudWatch.



