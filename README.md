# Azure Static Website Deployment

## Overview
This project demonstrates the deployment of a cloud-based static web application integrated with monitoring and alerting capabilities using Microsoft Azure.

## Objectives
- Deploy a static website on Azure  
- Enable logging for storage activities  
- Configure monitoring using Azure Monitor  
- Implement alert system for activity detection
  
## Architecture
User → Azure Storage → Azure Monitor → Alert Rule → Email Notification

## Technologies Used
- Microsoft Azure  
- Azure Storage Account  
- Azure Monitor  
- Azure Alerts  
- HTML 

## Implementation

### 1. Static Website Deployment
- Created Azure Storage Account  
- Enabled Static Website Hosting  
- Uploaded `cldweb.html` to `$web` container

### 2. Logging Configuration
- Enabled logging for storage operations:
  - Read  
  - Write  
  - Delete  
- Configured Blob service diagnostic settings

### 3. Monitoring Setup
- Used Azure Monitor to track activity  
- Selected **Transactions metric**  
- Configured threshold-based monitoring

### 4. Alert Configuration
- Created alert rule:
  - Condition: Transactions > 0  
- Configured Action Group:
  - Email notification  
- Linked alert rule to storage monitoring

### 5. Testing & Validation
- Uploaded and modified files in `$web` container  
- Alert triggered successfully  
- Email notification received

## Key Learnings
- Understanding of cloud storage and static hosting  
- Importance of logging and monitoring in cloud environments  
- Basic implementation of alert-based detection system  
- Hands-on experience with Azure service

## 👤 Author
Steven Ling
