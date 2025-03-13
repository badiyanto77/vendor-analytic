
# Vendor Monitoring Dashboard Project
The management stakeholder needs to have overview spending throughout the organization.
The tool provided enabling the identification of potential reduction cost through finding leverage among the vendors. 

# Introduction & Goals
The project demonstrates the process from data collection, data cleaning, data transformation, and data visualization. 
The project is developed using Azure data engineering platform, and utilize Power BI as tool to develop data visualization.

# Contents
- [The Architecture Diagram](#the-architecture-diagram)
- [The Data Set](#the-data-set)
- [Used Tools](#used-tools)
- [Pipelines](#pipelines)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Follow Me On](#follow-me-on)


# The Architecture Diagram
![Screenshot 2025-03-13 132848](https://github.com/user-attachments/assets/7d315c30-60da-4228-b4f8-90c7c0cdc503)



# The Data Set
The data sources is from transactional database resides on premise SQL Server database in the organization.
# Used Tools
- Azure Data Factory is used to create the entire pipeline and scheduling
- Databrick is used in data extraction and transformation process using python and spark script
- Datalake Gen2 is used to store data in bronze, silver and gold layer
- Azure Analytic Synapse is used to capture the transformed data and interfacing with data analytic tool
- Self Hosted Runtime Integration is used to connect on premise database server with Azure data engineering resource

# Pipelines
The pipeline design is divided into 3 phases :
- Extraction and Loading phase : collecting data from on premise database and store it in azure datalake bronze layer in parquet format
- Bronze to Silver transformation : transforming data format, standardize column name, and create date calendar dimension table
- Silver to Gold transformation : Tight couple all of the data ensuring only relevant data moved to the gold layer

# Visualization
Power BI is used as data visualization tool, due to the easy connectivity with azure platform. 

# Batch Processing
The batch processing is scheduled every day to obtain meaningful amount of data change 

# Transformed Data Model
![Screenshot 2025-03-13 124719](https://github.com/user-attachments/assets/1dcd3246-47b2-469b-84a4-2a5bcf64ede9)


# Conclusion
The project is straigh forward extracting and transforming data from on premise SQL server database which already in a good format since it is relational database. 

# Follow Me On
[My LinkedIn Profile](https://www.linkedin.com/in/bagus-adiyanto-29a9a229/)

