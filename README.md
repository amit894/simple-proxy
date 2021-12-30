# simple-proxy
Simple Proxy on Kubernetes

## PreRequisites

* Install python 3 on your machine : https://www.python.org/downloads/
* Installing Minikube on local: https://kubernetes.io/docs/tasks/tools/

## Running Minikube on Local

- ``` brew install minikube ```
- ``` minikube start ```
- ``` minikube status ```

## Installation

### Creating Deployments

- ``` cd resources/k8-manifests/deployments ```
- ``` kubectl apply -f . ```

### Creating Services

- ``` cd resources/k8-manifests/services ```
- ``` kubectl apply -f . ```

### Creating Ingress

- ``` cd resources/k8-manifests/ingress ```
- ``` kubectl apply -f . ```

### Enabling Tunnel

- ``` minikube tunnel ```


## Validating Deployments

- ``` curl -H “Host: rgate” “http://localhost/static-1/"  ```





