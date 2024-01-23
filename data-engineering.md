---
title: "What's new and planned for Synapse Data Engineering in Microsoft Fabric"
description: See what's new and planned for Synapse Data Engineering in Microsoft Fabric. Fabric Data Engineering release plans or roadmap.
ms.reviewer: sngun
ms.author: sngun
author: snehagunda
ms.topic: conceptual
ms.date: 10/04/2023
---

# What's new and planned for Synapse Data Engineering in Microsoft Fabric

> [!Important]
> The release plans describe functionality that may or may not have been released yet. The delivery timelines and projected functionality may change or may not ship. Refer to [Microsoft policy](https://go.microsoft.com/fwlink/p/?linkid=2007332) for more information.

Synapse Data Engineering empowers data engineers to be able to transform their data at scale using Spark and build out their lakehouse architecture. There are five key areas of Synapse Data Engineering that you can start using for your projects today: 

**Lakehouse for all your organizational data:** The lakehouse is a new item in Fabric that combines the best of the data lake and the data warehouse in a single experience. It enables users to ingest, prepare, and share organizational data in an open format in the lake. Later you can access it through multiple engines such as Spark, T-SQL, and Power BI. It provides various data integration options such as dataflows and pipelines, shortcuts to external data sources, and data product sharing capabilities.   

**Performant Spark engine & runtime:** Synapse Data engineering provides customers with an optimized Spark runtime with the latest versions of Spark (3.3.1), Delta (2.2), and Python (3.10). It uses Delta Lake as the common table format for all engines, enabling easy data sharing and reporting with no data movement. The runtime comes with Spark optimizations, enhancing your query performance without any configurations. It also offers starter pools and high-concurrency mode to speed up and reuse your Spark sessions, saving you time and cost. 

**Spark Admin & configurations:** Workspace admins with appropriate permissions can create and configure custom pools to optimize the performance and cost of their Spark workloads. They can also install libraries, select the runtime version, and set Spark properties to customize the Spark environment. These settings will apply to all notebooks and Spark jobs in the workspace, unless otherwise specified. 

**Developer Experience:** Developers can use notebooks, Spark jobs, or their preferred IDE to author and execute Spark code in Fabric. They can natively access the lakehouse data, collaborate with others, install libraries, track history, do in-line monitoring, and get recommendations from the Spark advisor. They can also use Data Wrangler to easily prepare data with a low-code UI. 

**Platform Integration:** All Synapse data engineering items, including notebooks, Spark jobs, pipelines, and lakehouses, are integrated deeply into the Fabric platform (enterprise information management capabilities, lineage, sensitivity labels, and endorsements). This integration will continue to deepen this semester with many new investments. 

Synapse Data Engineering in Microsoft Fabric is currently in public preview. To learn more, see the [documentation](/fabric/data-engineering/data-engineering-overview) and visit our [announcement blog](https://blog.fabric.microsoft.com/blog/category/announcements).

## Investment areas

| Feature       | Estimated release timeline |
| -------------- | -------------------------- |
| [Lakehouse data security (Public Preview)](#security)  | Q2 2024  |
| [Schema support for Lakehouse](#schema-support)| Q2 2024  |
| [Spark autotune (Public Preview)](#autotune)  | Q1 2024  |
| [High concurrency in pipelines](#concurrency)  | Q2 2024  |
| [Policy management](#policy)| Q2 2024 |
| [Environments (GA)](#environment) | Q2 2024 |
| [Notebooks in an app (Public Preview)](#notebook) | Q2 2024 |
| [Dynamic lineage of data engineering items](#data-lineage) | Q1 2024 |


### <a name="security"></a>Lakehouse data security (Public Preview) 

**Estimated release timeline: Q2 2024** 

You'll have the ability to apply file, folder, and table (or object level) security in the lakehouse. you can also control who can access data in the lakehouse, and the level of permissions they have. For example, You can grant read permissions on files, folders, and tables. Once permissions are applied, they're automatically synchronized across all engines. Which means, that permissions will be consistent across Spark, SQL, Power BI, and external engines.  

### <a name="schema-support"></a>Schema support for Lakehouse 

**Estimated release timeline: Q2 2024** 

The lakehouse will support 3-part naming convention. It enables you to add schemas to your lakehouses, which is consistent with the current warehouse experience. 

### <a name="autotune"></a>Spark autotune (Public Preview) 

**Estimated release timeline: Q1 2024** 

Autotune uses machine learning to automatically analyze previous runs of your Spark jobs and tunes the configurations to optimize the performance. It will configure how your data is partitioned, joined, and read by Spark. This way it will significantly improve the performance. We have seen customer jobs run 2x faster with this capability. 

### <a name="concurrency"></a>High concurrency in pipelines 

**Estimated release timeline: Q2 2024** 

In addition to high concurrency in notebooks, we will also enable high concurrency in pipelines. This capability will allow you to run multiple notebooks in a pipeline with a single session. 

### <a name="policy"></a>Policy management 

**Estimated release timeline: Q2 2024** 

Workspace admins will be able to author and enforce policies based on Spark properties, ensuring that your workloads comply with certain rules. For example, they can limit the number of resources, the time that a workload can consume, or prevent users from changing certain Spark settings. This will enhance the governance and security of your Spark workloads.  

### <a name="environment"></a>Create and attach environments (GA) 

**Estimated release timeline: Q2 2024** 

To customize your Spark experiences at a more granular level, you can create and attach environments to your notebooks and Spark jobs. In an environment, you can install libraries, configure a new pool, set Spark properties, and upload scripts to a file system. This gives you more flexibility and control over your Spark workloads, without affecting the default settings of the workspace. As part of GA, we are making various improvements to environments including API support and CI/CD integration.

### <a name="notebook"></a>Notebooks in an app (Public Preview) 

**Estimated release timeline: Q2 2024** 

You'll be able to embed your notebooks alongside Power BI reports and dashboards in Fabric apps and distribute them to business users. Customers will be able to interact with widgets and visuals in the notebook, as an alternative reporting and data exploration mechanism. This will enable you to create and share rich and engaging stories with your data. 

### <a name="data-lineage"></a>Dynamic lineage of data engineering items  

**Estimated release timeline: Q1 2024** 

You will be able to trace the lineage within Fabric across the code items such as notebooks & Spark jobs, and data items such as a lakehouse. This lineage will be dynamic, which means meaning if the code adds or removes references to lakehouses, it will be reflected in the lineage view. 

## Related content

- [Data Engineering documentation in Microsoft Fabric](/fabric/data-engineering/)
