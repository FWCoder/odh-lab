# OpenDataHub - Simple Lab
The content of this repo is designed to provide a simple scenario on how the Open Data Hub is installed. Usually based on your requirement, you may not need all components within Open Data Hub. When each user login into the OpenDataHub and start using each component, the resource will be consumed significantly. It is important to install what you need for your engagement. 

1. Follow the instruction on OpenDataHub Website to Install OpenDataHub Operator from Operator Hub and create an instance of ODH in your namespace
- https://opendatahub.io/docs/getting-started/quick-installation.html
2. Configure Kdef Yaml to only install the following items: 
	- JupyterHub
	- Seldon
	- Spark
	- Seldon
3. Validate if all components are started correctly on your environment
4. Follow the Basic Tutorial to validate if you can start up a simple notebook with Spark Cluster. (Avoid any Object Storage tutorial)
- https://opendatahub.io/docs/getting-started/basic-tutorial.html
6. From the Jupyter Notebook environment, open [Terminal] from [New] menu. 
7. Use `env` to explore how Jupyter Notebook connects with other component within Open Data Hub.
8. Reconfigure Spark Cluster from your laptop terminal using OpenShift Client 
- Find Spark Cluster object: `oc get SparkCluster`
- Edit your Spark Cluster to have only 1 worker node instead of 2: `oc edit SparkCluster <CLUSTER_NAME>`
9. Reran the Jupyter Notebook to validate if there is only one Spark Worker Node in your Cluster.