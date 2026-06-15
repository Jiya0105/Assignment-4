# Azure Cloud Fundamentals and Data Pipeline Implementation using Azure Data Factory

## Project Overview

This project demonstrates the implementation of a simple data pipeline using Microsoft Azure Cloud services. The pipeline uses Azure Blob Storage and Azure Data Factory (ADF) to read a CSV file, validate its metadata, and copy the data to another storage location.

The project was completed as part of a cloud computing assignment to understand Azure resource management and data integration services.

---

## Objective

The main objectives of this project are:

- Understand Microsoft Azure Cloud fundamentals.
- Create and manage Azure resources.
- Configure Azure Storage Accounts and Blob Containers.
- Build and execute a data pipeline using Azure Data Factory.
- Validate file metadata before processing.
- Transfer data between Blob Storage containers.

---

## Technologies Used

- Microsoft Azure Portal
- Azure Resource Groups
- Azure Storage Account
- Azure Blob Storage
- Azure Data Factory (ADF)
- Azure IAM (Identity and Access Management)
- CSV Dataset (Superstore Dataset)

---

## Project Workflow

### Step 1: Resource Group Creation

- Created a Resource Group in Azure Portal.
- Selected subscription and region.
- Used the Resource Group to organize all project resources.

### Step 2: Storage Account Setup

- Created an Azure Storage Account.
- Configured Standard Performance and LRS redundancy.
- Created Blob Storage containers.

### Step 3: Dataset Upload

- Downloaded the Superstore Dataset.
- Uploaded the CSV file into the source Blob container.

### Step 4: Azure Data Factory Configuration

- Created an Azure Data Factory instance.
- Explored Author, Monitor, and Manage sections.
- Created Linked Services for Azure Storage connectivity.

### Step 5: Dataset Configuration

Created:

- Source Dataset → Superstore.csv
- Destination Dataset → Processed_Superstore.csv

### Step 6: Metadata Validation

Used the **Get Metadata Activity** to verify:

- File existence
- File size
- Last modified date

### Step 7: Data Pipeline Development

Pipeline Structure:

Get Metadata → Copy Data → Destination File

Pipeline Name:

PL_Copy_Superstore_Data

### Step 8: Pipeline Execution

- Executed the pipeline using Debug and Trigger Now.
- Monitored execution in ADF Monitor.
- Verified output file generation.

### Step 9: IAM Role Assignment

Assigned:

- Reader Role
- Contributor Role
- Storage Blob Data Contributor Role

to ensure proper access control and storage connectivity.

---

## Mini Project

### Problem Statement

Create a complete Azure Data Factory pipeline that reads a CSV file from Azure Blob Storage, validates metadata, and copies the file to another storage location.

### Implementation

- Uploaded Superstore dataset to Blob Storage.
- Configured Linked Service.
- Created source and destination datasets.
- Added Get Metadata activity.
- Added Copy Data activity.
- Executed and monitored the pipeline.

### Output

- Source file detected successfully.
- Metadata validated successfully.
- Data copied to destination container.
- Pipeline execution status: Succeeded.

---

## Learning Outcomes

Through this project, I learned:

- Azure resource management
- Azure Blob Storage operations
- Linked Services and Datasets in ADF
- Metadata validation techniques
- Data movement using Copy Activity
- IAM role assignment and access control
- Pipeline monitoring and troubleshooting

---

---

## Dataset Used

Superstore Dataset (CSV Format)

---

## Conclusion

This project successfully demonstrated the implementation of a complete Azure data pipeline using Azure Storage and Azure Data Factory. The workflow included resource creation, storage configuration, metadata validation, data transfer, and access management. The project provided practical experience with Azure cloud services and strengthened understanding of data integration and pipeline execution in a cloud environment.
