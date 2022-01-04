# Cloud-Computing---Brain-Tumour-Classification
a project for Cloud Computing,  2021/2022,

The following resources could be deemed as either necessary or just useful for this project:
1.	Kaggle – Brain Tumor Dataset – the data files (.csv) were imported from here, plenty of ideas considering machine learning can be found there too:
https://www.kaggle.com/jakeshbohaju/brain-tumor/
2.	Udemy – Azure Databricks & Spark Core for Data Engineers course
https://www.udemy.com/course/azure-databricks-spark-core-for-data-engineers/
explanation of Azure Databricks/Delta Lake layout, configuration and basic operations in Spark 
3.	Apache Spark Documentation, especially Machine Learning Library:
https://spark.apache.org/docs/latest/ml-guide.html




Configuration:
•	Create an account (student license) on Azure platform (don’t use the WUT email address for account name as it will block your access to Active Directory)
•	Create a standard Databricks workspace
•	Create a Cluster, I mainly worked on a Standard F4s
•	Create an Azure DataLake Gen2 Storage account and at least one blob container, consider downloading a Storage Explorer
•	Create a Service Principal, register the application , copy the client, tenant IDs, create a new Client secret and copy its value, add a new role assignment storage account (storage blob container contributor).  Consider also creating a Key Vault in Azure where you write down the secrets, then in Databricks homescreen open the hidden UI by appending the address with #secrets/secretsScope and copy data from the key vault. 
•	Mount the new ADLS container in a databricks notebook using the ids and secrets you’ve saved, attach it to the cluster
•	Upload the dataset into your container
•	Create a new notebook, attach it to the cluster, and you’re set. 
