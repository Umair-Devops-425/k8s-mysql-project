<!-- # MySQL on Kubernetes (Minikube) -->
# MySQL on Kubernetes (Minikube)
A Kubernetes project that deploys MySQL with persistent storage, secrets, and services — all tested in Minikube.

<!-- ## Features -->
## Features
- PersistentVolume + PVC for database storage
- Secret to manage root password
- MySQL Deployment with 1 replica
- ClusterIP Service to expose MySQL
- Tested via CLI inside the pod

<!-- ## Getting Started -->
## Getting Started
1. Clone repo
2. Start Minikube
3. Apply manifests:

## 🔐 Note on Secrets
The `mysql-secret.yaml` file is excluded from this repo for security reasons.

To create the secret manually, run:

```bash
kubectl create secret generic mysql-secret \
  --from-literal=mysql-root-password='your-password'