# 🔄 Data Ingestion Pipeline in Microsoft Fabric

This repository documents the completion of a hands-on lab focused on building a **data ingestion pipeline** using Microsoft Fabric's native pipeline and notebook capabilities.

## 🎯 Purpose of the Lab

The primary goal of this lab was to demonstrate how to ingest data from external sources into a Fabric lakehouse using a combination of:
- **Pipelines** for orchestration and automation
- **Copy Data activities** for movement
- **Spark notebooks** for transformation and loading into tables

The exercise simulates a practical ETL/ELT use case, where sales data is fetched via HTTP, stored in OneLake, transformed, and loaded into Delta tables within a lakehouse.

## 🧠 What I Learned

By completing this lab, I gained experience with key data engineering features in Microsoft Fabric:

- **Workspace and Lakehouse Creation**  
  Learned how to set up a Fabric workspace and create a lakehouse structure to serve as the analytical data store.

- **Pipeline Development**  
  Built a pipeline that:
  - Deletes existing staging files
  - Copies new data from a public HTTP source
  - Triggers a Spark notebook to process and load data into a lakehouse table

- **Notebook Integration**  
  Created a parameterized Spark notebook that:
  - Reads raw data from the lakehouse file layer
  - Performs lightweight transformations (date fields, name splitting, column ordering)
  - Loads the output into a structured Delta table

- **End-to-End Automation**  
  Understood how to coordinate file management, ingestion, transformation, and loading in a repeatable, automated workflow.

- **Parameter Passing in Pipelines**  
  Used pipeline parameters to make the notebook dynamic and reusable across different tables.

## ✅ Outcome

At the end of this exercise, I successfully built a fully automated ETL pipeline that:
- Pulls sales data from an external HTTP source
- Cleans and transforms the data
- Loads it into a managed Delta table inside a Fabric lakehouse

This pipeline can now be reused or extended to process other data sources or additional transformation logic.

## 🤝 Let's Connect

If you’re working on modern data ingestion patterns with Microsoft Fabric or exploring lakehouse architectures, I’d love to connect and exchange ideas.  
Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/eyilan/) — let’s talk data and Fabric!
