## Overview
This repository hosts the `#ThreeTierAppChallenge`. 
The challenge involves deploying a Three-Tier Web Application using ReactJS, NodeJS, and MongoDB, with deployment on personal Kubernetes cluster using Minikube and managed the deployments using ArgoCD. Participants are encouraged to deploy the application, add creative enhancements, and submit a Pull Request (PR).

## Challenge Steps

### Step 1: Install Docker
``` shell
sudo apt-get update
sudo apt install docker.io
docker ps
sudo chown $USER /var/run/docker.sock
```

### Step 2: Install kubectl
``` shell
curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.19.6/2021-01-05/bin/linux/amd64/kubectl
chmod +x ./kubectl
sudo mv ./kubectl /usr/local/bin
kubectl version --short --client
```

### Step 3: Run Manifests
``` shell
kubectl apply -f .
kubectl delete -f .
```

### Step 4: Install ArgoCD
``` shell
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

## Contribution Guidelines
- Fork the repository and create your feature branch.
- Deploy the application, adding your creative enhancements.
- Ensure your code adheres to the project's style and contribution guidelines.
- Submit a Pull Request with a detailed description of your changes.

## Support
For any queries or issues, please open an issue in the repository.

---
Happy Coding! 🚀👨‍💻👩‍💻
