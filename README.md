# managed_airflow

The purpose of this repository is to create a managed, production ready, minimal maintenance Airflow installation in AWS.

The components that can be created from this repo are:
* Kubernetes Cluster running on EKS with Fargate
* Managed PostgreSQL database running on AWS RDS
* Airflow webserver, scheduler and Kubernetes Executor docker images
* NFS for sharing DAGs with the cluster, backed by AWS EFS
* Related configurations

