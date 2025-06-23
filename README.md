# azure-billing-cost-optimization
Azure serverless cost optimization solution using Cosmos DB and Blob Storage

# Azure Billing Cost Optimization

This solution offloads rarely accessed billing records from Cosmos DB to Azure Blob Storage using Azure Functions. It reduces storage and read costs while maintaining data availability and API compatibility.

## Architecture
![Architecture Diagram](architecture-diagram.png)

## Functions
- archive-function: Moves old records to blob
- proxy-function: Reads from blob if record not in Cosmos DB

## Tech Used
Azure Functions, Cosmos DB, Blob Storage, FastAPI, Python

