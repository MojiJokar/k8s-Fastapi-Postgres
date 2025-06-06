# k8s-Fastapi-Postgres
# Deployment using Kubernetes' standard YAML files, to deploy with  the Namespace "standard"
here there are  Deliverables:
- A YAML-STANTARD directory with all the configurations.

- The log files for  various microservices (FastAPI, PostgreSQL).

- A backup file of your ETCD database once all the configurations set up have been deployed.

# Description:
- Kubernetes (or K8s) is an open source container orchestrator maintained by the Cloud Native Computing Foundation (CNCF). Thanks to its highly advanced features and large number of contributors, Kubernetes has become a de facto standard over time, supplanting Mesos and Docker Swarm, for example. As a DevOps engineer, getting to grips with Kubernetes and implementing it is essential.

 In this project:
 
 there are microservices which  manage their lifecycle, and set up administrative tasks like backing up and restoring  Cluster, we deploy new microservices that will enable the registration and counting of users present on this platform.
 
 # there are  2 microservices to deploy:

- a service that will deploy your FastAPI application.
-  second service that will deploy your PostgresSQL database.

  # RoadMap

Define the appropriate Kubernetes objects for optimal deployment of microservices, we can choice for the type of object to use.

Write the Dockerfile for the microservice FastAPI. The application is available on the following repository: kubernetes-devops-project.git.

the docker-compose.yaml file in order to understand the architecture to be deployed.


You will use Rancher's default storage class (StorageClass) to manage your storage for your application. Your storage volume will have 10 Gb of storage and should allow multiple Pods to write to it.

 3 replicas of your application when it is deployed.

 a backup plan for your cluster using the K3s client.

All tasks will need to be set up in this way:

# A few tips to get started:

- Each microservice will need to be exposed via a service so that other microservices can connect to a specific port.

- The only Pod with which we will be able to connect via ingress is that of the FastAPI application.

- Choosing  type of application (Stateful, Stateless) is importantn or according to confidentiality (ConfigMap, Secret)

- To populate the  database you can do this on the /docs route of your micro-service FastAPI.

- For the list of users, the route is /users.

- For the count of all users on the platform, the route is /users/count.

  
