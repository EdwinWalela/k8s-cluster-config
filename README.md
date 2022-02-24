# Kubernetes Demo Cluster Configuration

Configuration files for SAAS architecture 

Consists of deployments, services and configMaps for a [demo K8s cluster](https://github.com/EdwinWalela/k8s-cluster) running on minikube.

## Requirements

- kubectl
- minikube

## Setup

- clone repo

- `minikube start`

### Create namespaces

- `cd namespace`

- `kubectl apply -f .`


### Create client instances

- `cd client-a`

- `kubectl apply -f . -R`

- `cd client-b`

- `kubectl apply -f . -R`


## Deployments

Run `kubectl get deployment -n client-a`


Run `kubectl get deployment -n client-b`

Created deployments

- Blog (Laravel)
- API (Golang)
- PhpMyAdmin
- MySQL (DB)

## Access applications

List avaiable services 

`kubectl get services -n client-a`

`kubectl get services -n client-b`

### Assign external IP addresses to services

`minikube service blog -n client-a` 

`minikube service goapi -n client-a` 

`minikube service phpmyadmin -n client-a` 


