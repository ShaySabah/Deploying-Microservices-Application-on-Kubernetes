# Deploying-Microservices-Application-on-Kubernetes
Deploying-Microservices-Application-on-Kubernetes
# Microservices Application Deployment on Kubernetes with Minikube

This repository contains YAML configurations to deploy a microservices application on Kubernetes using Minikube and `kubectl` command-line tools.

![image](https://github.com/ShaySabah/Deploying-Microservices-Application-on-Kubernetes/assets/139687184/4c1049c0-3100-4517-b8da-0acc1ab7fefa)

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

![WhatsApp Image 2024-02-25 at 11 30 33](https://github.com/ShaySabah/Deploying-Microservices-Application-on-Kubernetes/assets/139687184/3096d64b-8a6e-4b79-bc1b-4297a8ac6f12)


Application URLs
Voting App: http://localhost:30004
Result App: http://localhost:30005
