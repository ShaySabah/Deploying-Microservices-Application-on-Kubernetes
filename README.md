# Deploying-Microservices-Application-on-Kubernetes
Deploying-Microservices-Application-on-Kubernetes
# Microservices Application Deployment on Kubernetes with Minikube

This repository contains YAML configurations to deploy a microservices application on Kubernetes using Minikube and `kubectl` command-line tools.

## Overview

This microservices application consists of several components:

- **Voting App**: A component allowing users to vote.
- **Redis**: Used as a message broker between the Voting App and Worker App.
- **Worker App**: Processes the votes received from the Voting App.
- **Postgres**: Database for storing vote results.
- **Result App**: Displays the aggregated voting results.

## Prerequisites
Ensure the following software is installed:

- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

## Deployment Steps

### 1. Voting App

```bash
kubectl apply -f voting-app.yaml
Access the Voting App at http://localhost:30004

2. Redis
bash
Copy code
kubectl apply -f redis.yaml
3. Worker App
bash
Copy code
kubectl apply -f worker-app.yaml
4. Postgres
bash
Copy code
kubectl apply -f postgres.yaml
5. Result App
bash
Copy code
kubectl apply -f result-app.yaml
Access the Result App at http://localhost:30005

Application URLs
Voting App: http://localhost:30004
Result App: http://localhost:30005
