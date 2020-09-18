# OpenDataHub - Simple Lab
The content of this repo is designed to provide a simple scenario on how the Open Data Hub is installed. Usually based on your requirement, you may not need all components within Open Data Hub. When each user login into the OpenDataHub and start using each component, the resource will be consumed significant. It is important to install what you need for your engagement. 

1. Install OpenDataHub Operator from Operator Hub
2. Create instance of ODH in your namespace
3. Configure Kdef Yaml to only install the following items: 
	- JupyterHub
	- Seldon
	- Grafana
	- Spark
	- Prometheus
4. Validate if all components are started correctly on your environment
