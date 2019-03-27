# [Proctor Guide] Challenge 01 - Prepare Resources

## Azure Subscription

Please encourage teamwork throughout and remind teams that most of the resources to deploy are one per team, not one per person.

Teams can work in one person’s subscription and use RBAC to add other team members. The same applies in Databricks – encourage teams to work in the Shared area of the workspace and for the cluster owner to add others to the workspace.

## Tooling
If teams do not have the tools installed on their laptops already, then they can either download/install them or consider deploying an Azure Data Science VM (DSVM) instance, which has all of the tools installed already.

## Storage Account
Teams should use GP v2 storage accounts. LRS is fine for the hack.

## Azure Databricks
ADB Premium cluster is required.

No special Databricks configuration is needed. No GPU or ML support is needed. Defaults will generally work well.

## References

Spark configuration: <https://docs.azuredatabricks.net/user-guide/clusters/spark-config.html#spark-config>

Accessing Azure Storage from Databricks: <https://docs.azuredatabricks.net/spark/latest/data-sources/azure/azure-storage.html>

## Azure Data Factory

Create an Azure Data Factory V2 project. You do not need an SSIS IR.

## Azure SQL Data Warehouse

Deploy an Azure SQL Data Warehouse instance. Either gen 1 or gen 2 is fine.

## Azure Analysis Service

Create Azure Analysis Services project.

## Azure Cosmos DB

Deploy an Azure Cosmos DB instance. Minimum specs (single partition, 10GB, 400RU) are fine for this event.

## Azure Functions App

Deploy an Azure Functions App. Defaults are fine. Either model (Consumption or App Service) is fine.