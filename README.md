# Kubernetes Demo Cluster Configuration

Configuration files for deployments, services and configMaps for a demo K8s cluster.

## Setup

- `minikube start`

- `kubectl apply -f .`

## Deployments

Run `kubectl get deployment`

Created deployments

- Blog (Laravel)
- API (Golang)
- PhpMyAdmin
- MySQL (DB)

## Accessible services

List avaiable services using  `kubectl get services `

- `minikube service blog` Asssigns external IP to blog
- `minikube service goapi` Assigns external IP to API
- `minikube service phpmyadmin` Assigns external IP to phpmyadmin

