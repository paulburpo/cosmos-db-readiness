# Cosmos DB Readiness Guide

This document is a collection of Cosmos DB resources across the different areas of Microsoft documentation. If you are looking for more of a classic training course, take a look at the Cosmos DB workshop in the "*Labs, Workshops and Hackathons*" section below.

# Understanding Cosmos DB

The purpose of this section is to give you a basic understanding of Cosmos DB including what Cosmos DB is, architectural patterns, use cases and management tools.

[Introduction to Cosmos DB](https://docs.microsoft.com/azure/cosmos-db/introduction)

## What is NoSQL?

Understanding Cosmos DB starts by understanding relational and the various non-relational data models. 

- [Understanding the differences between NoSQL and relational databases](https://docs.microsoft.com/en-us/azure/cosmos-db/relational-nosql)
- [Non-relational data and NoSQL](https://docs.microsoft.com/en-us/azure/architecture/data-guide/big-data/non-relational-data)

## Choosing an appropriate data store in Azure

When architecting data solutions in Azure, you have many data platforms to choose from. Understanding when to use a particular data platform will help you build highly resilient and scalable solution in Azure. 

- [Use the best data store for the job (polyglot persistance)](https://docs.microsoft.com/en-us/azure/architecture/guide/design-principles/use-the-best-data-store)
- [Understand data store models](https://docs.microsoft.com/en-us/azure/architecture/guide/technology-choices/data-store-overview)
- [Select a data store](https://docs.microsoft.com/en-us/azure/architecture/guide/technology-choices/data-store-decision-tree)
- [Criteria for choosing a data store](https://docs.microsoft.com/en-us/azure/architecture/guide/technology-choices/data-store-considerations)
- [Choosing an analytical data store in Azure](https://docs.microsoft.com/en-us/azure/architecture/data-guide/technology-choices/analytical-data-stores)
- [Choosing a big data storage technology in Azure](https://docs.microsoft.com/en-us/azure/architecture/data-guide/technology-choices/data-storage)

## Architectural Patterns with Cosmos DB 

- [Tenancy models for SaaS applications](https://docs.microsoft.com/en-us/azure/architecture/isv/application-tenancy)
- [Common Azure Cosmos DB use cases](https://docs.microsoft.com/azure/cosmos-db/use-cases)
- [Browse Azure Architecture](https://docs.microsoft.com/en-us/azure/architecture/browse/?terms=Cosmos%20DB), Azure Architectures that leverage Cosmos DB from the Azure Architecture Center. You can leverage these as a starting point for your solutions.

## Management Tools for Cosmos DB

- [Storage Explorer](https://docs.microsoft.com/azure/cosmos-db/storage-explorer)
- [Cosmos DB Data Explorer](https://docs.microsoft.com/azure/cosmos-db/data-explorer)

## Other Resources
- [Demo and Query Playground](https://www.documentdb.com/sql/demo), useful for understanding how to query without having to provision a Cosmos DB account.

# Implementing Cosmos DB

This section covers the core concepts around implementing Cosmos DB.

## Provisioning and Pricing

- [Account Creation and Failover](https://docs.microsoft.com/azure/cosmos-db/how-to-manage-database-account)
- [Backup and Restore](https://docs.microsoft.com/azure/cosmos-db/online-backup-and-restore)
- [Pricing model](https://docs.microsoft.com/azure/cosmos-db/how-pricing-works)
- [Request Units](https://docs.microsoft.com/azure/cosmos-db/request-units)
- [RU Calculator](https://cosmos.azure.com/capacitycalculator/)
- [Reserved Instances](https://docs.microsoft.com/azure/billing/billing-understand-cosmosdb-reservation-charges)
- [Provisioned Throughput, Not Capacity](https://docs.microsoft.com/azure/cosmos-db/set-throughput)
- [Provision Autoscale Throughput](https://docs.microsoft.com/azure/cosmos-db/provision-throughput-autoscale)
- [How to choose between standard and autoscale provisioned throughput](https://docs.microsoft.com/azure/cosmos-db/how-to-choose-offer)
- [Optimizing Query Cost](https://docs.microsoft.com/azure/cosmos-db/optimize-cost-queries)
- [Optimizing Storage Cost](https://docs.microsoft.com/azure/cosmos-db/optimize-cost-storage)
- [Using as a Key Value Store - Costs](https://docs.microsoft.com/azure/cosmos-db/key-value-store-cost)

## Resource Model

- [Cosmos DB Resource Model](https://docs.microsoft.com/en-us/azure/cosmos-db/account-databases-containers-items)
- [Indexes](https://docs.microsoft.com/en-us/azure/cosmos-db/index-overview)
- [Time to Live (TTL)](https://docs.microsoft.com/azure/cosmos-db/time-to-live)
- [Unique key constraints](https://docs.microsoft.com/en-us/azure/cosmos-db/unique-keys)
- [Attachments](https://docs.microsoft.com/en-us/azure/cosmos-db/attachments)

## Global Distribution

- [Consistency Tradeoffs](https://docs.microsoft.com/azure/cosmos-db/consistency-levels-tradeoffs)
- [High Availability](https://docs.microsoft.com/azure/cosmos-db/high-availability)
- [Multi-Master Replication](https://docs.microsoft.com/azure/cosmos-db/how-to-multi-master)
- [Consistency Levels](https://docs.microsoft.com/azure/cosmos-db/how-to-manage-consistency)
- [Conflict Resolution Policies](https://docs.microsoft.com/en-us/azure/cosmos-db/conflict-resolution-policies)
- [Cosmos DB Internal Architecture](https://docs.microsoft.com/en-us/azure/cosmos-db/global-dist-under-the-hood)

## Integration with other Azure Services

- [Synapse Link](https://docs.microsoft.com/azure/cosmos-db/synapse-link)
- [Change Feed](https://docs.microsoft.com/azure/cosmos-db/change-feed)
- [Integration with Azure Cognitive Search](https://docs.microsoft.com/azure/search/search-howto-index-cosmosdb)
- [Functions Integration](https://docs.microsoft.com/azure/azure-functions/functions-bindings-cosmosdb-v2)
- [Debugging Cosmos and Azure Functions](https://docs.microsoft.com/azure/cosmos-db/troubleshoot-changefeed-functions)

## Security

- [CosmosDB Security](https://docs.microsoft.com/azure/cosmos-db/database-security)
- [Keys and Tokens](https://docs.microsoft.com/azure/cosmos-db/secure-access-to-data)
- [IP Firewall](https://docs.microsoft.com/azure/cosmos-db/firewall-support)
- [Cosmos DB Private Endpoints and Private Link](https://docs.microsoft.com/azure/cosmos-db/how-to-configure-private-endpoints)
- [Securing Cosmos Keys using Key Vault](https://docs.microsoft.com/azure/cosmos-db/access-secrets-from-keyvault)

# Data Modeling for Cosmos DB

This section covers partitioning and data modeling. Data modeling is one of the most critical aspects because of it's impact on performance. It is also one of the areas that customers struggle with the most.

## Partitioning
- [Partitioning and Horizontal Scaling](https://docs.microsoft.com/azure/cosmos-db/partition-data)
- [Large Partition Keys](https://docs.microsoft.com/azure/cosmos-db/large-partition-keys)

## Data Modeling
- [Social media use case with Cosmos DB](https://docs.microsoft.com/azure/cosmos-db/social-media-apps), provides a good data modeling walkthrough. 
- [Data Modeling](https://docs.microsoft.com/azure/cosmos-db/modeling-data)
- [Data Modeling - Real World Example](https://docs.microsoft.com/azure/cosmos-db/how-to-model-partition-example)

# Programming and Querying for Cosmos DB

This section covers programming, querying and performance tuning.

## Performance Tuning 
- [Tracking RU Charges](https://docs.microsoft.com/azure/cosmos-db/find-request-unit-charge)
- [Tuning Query Performance](https://docs.microsoft.com/azure/cosmos-db/sql-api-query-metrics)
- [Indexing Policies](https://docs.microsoft.com/azure/cosmos-db/index-policy)

## Development
- [Server Side Programming in CosmosDB](https://docs.microsoft.com/azure/cosmos-db/stored-procedures-triggers-udfs)
- [.Net core and SQL API](https://docs.microsoft.com/azure/cosmos-db/sql-api-sdk-dotnet-core)
- [JavaScript and SQL API](https://docs.microsoft.com/azure/cosmos-db/javascript-query-api)

## Other Useful Resources
- [Cosmos DB Query Cheat Sheets](https://docs.microsoft.com/azure/cosmos-db/query-cheat-sheet)
- [Troubleshooting .NET SQL SDK](https://docs.microsoft.com/azure/cosmos-db/troubleshoot-dot-net-sdk)
- [Scale Up a Collection command in .NET](https://docs.microsoft.com/dotnet/api/microsoft.azure.documents.client.documentclient.replaceofferasync?view=azure-dotnet)
- [Bulk Executor](https://docs.microsoft.com/azure/cosmos-db/bulk-executor-overview)
- [Cosmos DB Live Data Migrator](https://github.com/Azure-Samples/azure-cosmosdb-live-data-migrator)

# Labs, Workshops and Hackathons

- [Cosmos DB Workshop](https://azurecosmosdb.github.io/labs/). This workshop provides hands-on experience working with Cosmos DB. It targets the SQL API (using both .NET and Java), Gremlin and Cassandra. The labs cover a wide variety of core topics including provisioning, data import, querying, indexing, multi-document transactions, transactional continuation, change feed, performance troubleshooting and concurrency control.

- [IoT Scenario](https://github.com/AzureCosmosDB/scenario-based-labs/tree/master/IoT). In this lab, you will use Azure Cosmos DB to ingest streaming vehicle telemetry data as the entry point to a near real-time analytics pipeline built on Cosmos DB, Azure Functions, Event Hubs, Azure Databricks, Azure Storage, Azure Stream Analytics, Power BI, Azure Web Apps, and Logic Apps.

- [E-Commerce Scenario](https://github.com/AzureCosmosDB/scenario-based-labs/tree/master/Retail). In this lab, you you will implement a recommendation system for e-commerce using several Microsoft Azure services including Cosmos DB, Azure Functions, Event Hubs, Azure Databricks, Azure Storage, Azure Stream Analytics, Power BI, Azure Web Apps, and Logic Apps.

- [CosmicWorks](https://github.com/AzureCosmosDB/CosmicWorks). How to migrate a relational data model to Azure Cosmos DB.

- [Cloud Workshop - Cloud-native Applications](https://github.com/microsoft/MCW-Cloud-native-applications). In this workshop, you will build a proof of concept (POC) that will transform an existing on-premises application to a container-based application. This POC will deliver a multi-tenant web app hosting solution leveraging Azure Kubernetes Service (AKS), Docker containers on Linux nodes, and a migration from MongoDB to CosmosDB.

- [Cloud Workshop - Cosmos DB Real-time Advanced Analytics](https://github.com/Microsoft/MCW-Cosmos-DB-Real-Time-Advanced-Analytics). In this workshop, you will implement solutions that leverage the strengths of Cosmos DB in support of advanced analytics solutions that require high throughput ingest, low latency serving and global scale in combination with scalable machine learning, big data and real-time processing capabilities.

- [Cloud Workshop - Innovate and Modernize Apps with Data and AI](https://github.com/microsoft/MCW-Innovate-and-modernize-apps-with-Data-and-AI). In this workshop, you will build an IoT solution for data ingestion and predictive maintenance leveraging event sourcing and CQRS architectural patterns.

- [Cloud Workshop - Serverless Architecture](https://github.com/microsoft/MCW-Serverless-architecture). In this workshop, you will implement an end-to-end scenario using a supplied sample that is based on Microsoft Azure Functions, Azure Cosmos DB, Event Grid, and related services. The scenario will include implementing compute, storage, workflows, and monitoring, using various components of Microsoft Azure.

- [OpenHack - App Modernization with NoSQL](https://openhack.microsoft.com) The NoSQL OpenHack challenges developers and data professionals to migrate a legacy database application to a cloud-based NoSQL environment. Participants will scale the NoSQL solution for global availability and develop new functionality to provide additional insights to the business and value to customers.

- [OpenHack - Serverless](https://openhack.microsoft.com) During the Serverless OpenHack developers will explore how to quickly build and deploy Azure Serverless (Functions, Logic Apps, Event Grid & Cosmos DB) solutions. 
