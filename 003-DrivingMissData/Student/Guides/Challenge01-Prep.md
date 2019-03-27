# Challenge 01 - Prepare Resources

## Summary

Each Challenge will require certain resources, and you will need to make some decisions. Most of the Azure resources used in the Challenges are very quick to deploy.

However, some resources you will need will take longer to deploy. These are summarized in this document so that you can start them deploying while your team considers the to-do challenges.

## Azure Subscription

Resources in this hack need to be deployed into a pay-as-you-go or MSDN subscription. Trial or free subscriptions will not work.

The following resources should all be deployed in the same subscription. As a team, please consider how best to work together on resources for the duration of the hack.

## Tooling

You will need the following tools:

* Power BI Desktop

    Download: <https://powerbi.microsoft.com/desktop/>

* SQL Server Management Studio (SSMS)

    Download: <https://docs.microsoft.com/sql/ssms/download-sql-server-management-studio-ssms>

* SQL Server Data Tools (SSDT)

    Download: <https://docs.microsoft.com/sql/ssdt/download-sql-server-data-tools-ssdt>

* Azure Storage Explorer (recommended) or AzCopy

    Download: <http://storageexplorer.com/>

    Download: <https://aka.ms/downloadazcopy>

The installers for these are also available in the Teams channel for this event, in the Files area.

If you have these installed already on your computer, you can use them there.

If not, please install them - or consider using a Windows 2016 Data Science Virtual Machine (DSVM), which has Power BI Desktop and SSMS as well as the base SSDT as part of Visual Studio 2017 – though you will still need to install the extra SSDT tooling for SQL Analysis Services (see third link above).

## Storage Account

Create a storage account for data storage. You will later configure other resources to connect to this storage.

Note storage account region, name, key(s), and container name(s) for later use.

## Azure Data Factory

Create an Azure Data Factory V2 project. You do not need an SSIS IR.

## Azure Databricks

Deploy a Premium Azure Databricks service. When deployment completes, launch the workspace portal.

Create a new cluster. You do not need ML or GPU support for this hack. You can use the latest released version of Databricks (4.3 at the time of this writing).

## Azure SQL Data Warehouse

Deploy an Azure SQL Data Warehouse instance. Either gen 1 or gen 2 is fine.

## Azure Analysis Service

Create Azure Analysis Services project.

## Azure Cosmos DB

Deploy an Azure Cosmos DB instance. Minimum specs (single partition, 10GB, 400RU) are fine for this event.

## Azure Functions App

Deploy an Azure Functions App. Defaults are fine. Either model (Consumption or App Service) is fine.
