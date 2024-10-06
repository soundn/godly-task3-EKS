# gudlyf-task3-EKS

This project sets up an Amazon EKS cluster with a microservice application running in multiple namespaces. The EKS cluster is configured with auto-scaling based on custom metrics using Kubernetes Horizontal Pod Autoscaler (HPA) and Prometheus/Grafana for monitoring.

## Structure

- `terraform/`: Terraform code for creating the EKS cluster
- `helm/`: Helm charts for Prometheus and Grafana
- `kubernetes/`: Kubernetes manifests for deployments, services, and HPAs
- `scripts/`: Utility scripts for deployment and setup

## Setup

1. Create EKS cluster:
   ```
   cd terraform
   terraform init
   terraform apply
   ```

## Monitoring

Access Grafana dashboard at: 

## Autoscaling

The application uses HPA for autoscaling based on custom metrics. See `app-service-HPA-deploy-EKS/hpa/hpa.yml` for details.