## Lab 0: [Set up your Azure Databricks environment](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/00-setup.html)

Provision an Azure Databricks Premium workspace in your Azure subscription using Azure Cloud Shell.

- Duration: 15 minutes
- To learn more, visit [this](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/) learn module.
- Supporting notebook can be viewed [here](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/).

Notes:

✅ All good

---

## Lab 1: [Explore Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/01-explore-azure-databricks.html)

In this lab, you explore the Azure Databricks workspace UI, upload a sample dataset to a Unity Catalog volume, and work with notebook features including Python, SQL magic commands, and Markdown. You use Genie Code throughout to generate and refine code in the context of CityMoves Transit, a fictional public transportation authority.

- Duration: 30 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/modules/explore-azure-databricks/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/01-explore-azure-databricks.ipynb).

Notes:

✅ All good

---


## Lab 2: [Select and Configure Compute in Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/02-select-and-configure-compute.html)

In this lab, you create and configure an all-purpose cluster in Azure Databricks, install libraries both cluster-scoped and notebook-scoped, and use the faker library to generate and analyze synthetic patient admission records with PySpark.

- Duration: 30 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/select-and-configure-compute/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/02-select-and-configure-compute.ipynb).


Notes:

✅ Create tables routes

❌ Compute not available on free tier

Ref:
https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/upgrade-azure-subscription
https://www.reddit.com/r/databricks/comments/1c6anq6/databricks_free_trial_experience_your_feedback_is/


---


## Lab 3: [Create and organize objects in Unity Catalog](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/03-create-and-organize-objects-in-unity-catalog.html)

In this lab, you build a complete Unity Catalog namespace for a university data platform — creating a catalog, medallion schemas, managed tables with primary and foreign key constraints, views, a volume, and a reusable SQL function. You practice DDL operations such as adding columns and applying governance tags, and explore how Unity Catalog organizes and governs structured data at every layer of the medallion architecture. By the end, you will have a fully structured, query-ready environment that reflects real-world data engineering practices on Azure Databricks.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/create-and-organize-objects-in-unity-catalog/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/03-create-and-organize-objects-in-unity-catalog.ipynb).



Notes:

✅ Create tables university related

❌ Views - pre-computing: need compute serverfull - Data Wharehouse SQL - interessting notion 

Ref:

*The proximate error in Cell 21: Create departm... is MATERIALIZED_VIEW_OPERATION_NOT_ALLOWED. The root cause is not the SQL statement itself — it’s that the notebook is running on Serverless interactive compute, and this workspace is not enabled to create or refresh materialized views from that compute type. Because of that platform restriction, editing only this cell cannot make CREATE OR REFRESH MATERIALIZED VIEW succeed here without changing the task’s logic.*

*I did not rewrite the cell to a different object type because that would change the intended behavior. The correct approach is to run this same statement on a SQL warehouse, or use a workspace where materialized views are enabled for this compute. If you want a code-only workaround in this notebook, I can replace it with a regular view or a table build instead, but that would be a different result than a materialized view.*


---

## Lab 4: [Secure Unity Catalog objects](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/04-secure-unity-catalog-objects.html)

In this lab, you secure Unity Catalog objects in Azure Databricks by granting fine-grained access control to a Databricks group, applying row filters to restrict customer data by region, and masking PII email addresses using column mask functions. You also create an Azure Key Vault-backed secret scope and retrieve secrets securely inside a notebook, so sensitive credentials are never exposed in code.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/secure-unity-catalog-objects/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/04-secure-unity-catalog-objects.ipynb).


Notes:

On Going

---


## Lab 5: [Govern Unity Catalog objects](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/05-govern-unity-catalog-objects.html)

In this lab, you apply Unity Catalog governance controls to a connected vehicle data platform built on Azure Databricks. You use SQL to tag tables and columns for PII classification, configure Delta Lake retention policies and run VACUUM to purge deleted data, and enable predictive optimization. You then query system tables to trace data lineage programmatically and analyse the audit log to answer compliance questions about who accessed data and when.

- Duration: 30 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/govern-unity-catalog-objects/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/05-govern-unity-catalog-objects.ipynb).

## Lab 6: [Design and implement data modeling with Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/06-design-implement-data-modeling-unity-catalog.html)

In this lab, you design and implement a Delta Lake data model in Unity Catalog for a retail banking scenario, building a customer dimension with SCD Type 2 history tracking and a transaction fact table with liquid clustering. You apply Change Data Feed to build a queryable FCA compliance audit trail and use Delta Lake time travel to inspect and restore previous table versions.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/design-implement-data-modeling-unity-catalog/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/06-design-implement-data-modeling-unity-catalog.ipynb).

## Lab 7: [Ingest data into Unity Catalog](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/07-ingest-data-into-unity-catalog.html)

In this lab, you practise the core data ingestion techniques available in Azure Databricks. You load CSV files from a Unity Catalog managed volume into Delta tables using PySpark DataFrames, SQL COPY INTO, and CREATE TABLE AS SELECT. You also configure Auto Loader to automatically detect and process new files from cloud storage, demonstrating exactly-once ingestion for continuously arriving data.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/ingest-data-into-unity-catalog/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/07-ingest-data-into-unity-catalog.ipynb).

## Lab 08: [Cleanse, transform, and load data into Unity Catalog](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/08-cleanse-transform-load-data-into-unity-catalog.html)

In this lab, you clean and reshape raw real estate data in Azure Databricks. You choose the right data types for prices and timestamps, remove duplicate listings and fill missing values using PySpark, and combine data across tables with inner and left joins. You also use SQL PIVOT and UNPIVOT to restructure market statistics for trend analysis.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/cleanse-transform-load-data-into-unity-catalog/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/08-cleanse-transform-load-data-into-unity-catalog.ipynb).

## Lab 09: [Implement and Manage Data Quality Constraints in Unity Catalog](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/09-implement-manage-data-quality-constraints-unity-catalog.html)

In this lab, you build a Lakeflow Spark Declarative Pipeline for ClearCover Insurance that enforces data quality constraints on raw claims data. You implement nullability and range checks using pipeline expectations, validate data types with col().cast(), and handle schema drift using Auto Loader’s rescued data column. You then create and run the pipeline in the Databricks UI and monitor data quality metrics.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/implement-manage-data-quality-constraints-unity-catalog/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/09-implement-manage-data-quality-constraints-unity-catalog.ipynb).

## Lab 10: [Design and implement data pipelines with Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/10-design-implement-data-pipelines.html)

In this lab, you build a medallion architecture pipeline (Bronze → Silver → Gold) for GlobStay hotel booking data, applying cleaning rules such as deduplication, null filtering, and date validation before producing Gold-layer aggregations for property and channel performance. You implement error handling and parameterize notebooks for job orchestration. You then configure a Lakeflow Job in the Azure Databricks UI with sequential task dependencies, retry policies, failure notifications, and an If/else condition task for data quality routing.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/design-implement-data-pipelines/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/10-design-implement-data-pipelines.ipynb).

## Lab 11: [Implement Lakeflow Jobs with Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/11-implement-lakeflow-jobs.html)

In this lab, you configure and automate a CDR data pipeline for TelConnect using Lakeflow Jobs. You run a pre-built parameterized notebook that processes Call Detail Records through bronze, silver, and gold layers, then configure a Lakeflow Job in the Azure Databricks UI with task dependencies, a job parameter, scheduled and event-based triggers, failure notifications, and retry policies.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/implement-lakeflow-jobs/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/11-implement-lakeflow-jobs.ipynb).

## Lab 12: [Implement Development Lifecycle Processes in Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/12-implement-development-lifecycle-processes-in-azure-databricks.html)

In this lab, you implement a testing strategy for a data transformation pipeline using pytest, then package and deploy the pipeline as a Declarative Automation Bundle using the Databricks CLI.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/implement-development-lifecycle-processes-in-azure-databricks/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/12-implement-development-lifecycle-processes-in-azure-databricks.ipynb).

## Lab 13: [Monitor, Troubleshoot, and Optimize Workloads in Azure Databricks](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/13-monitor-troubleshoot-optimize-workloads-azure-databricks.html)

In this lab, you generate synthetic workloads with intentional data skew and excessive shuffle, use the Spark UI to diagnose the performance problems, and apply targeted fixes using broadcast joins, Adaptive Query Execution, and shuffle reduction techniques.

- Duration: 45 minutes
- To learn more, visit [this](https://learn.microsoft.com/training/wwl-databricks/monitor-troubleshoot-optimize-workloads-azure-databricks/) learn module.
- Supporting notebook can be viewed [here](https://github.com/MicrosoftLearning/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/blob/main/Allfiles/13-monitor-troubleshoot-optimize-workloads-azure-databricks.ipynb).

## Lab 0: [Clean up your Azure Databricks environment](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/Instructions/Labs/99-cleanup.html)

Clean up your resources in Azure using Azure Cloud Shell.

- Duration: 5 minutes
- To learn more, visit [this](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/) learn module.
- Supporting notebook can be viewed [here](https://microsoftlearning.github.io/DP-750T00-Implement-Data-Engineering-Solutions-using-Azure-Databricks/).