# My Kubernetes Application

This repository contains the manifests and configuration files for deploying a sample application on Google Kubernetes Engine (GKE).

## Live URL

The application is deployed and accessible at the following URL:

[http://34.28.182.11:80](http://34.28.182.11:80)

## Kubernetes Manifests

The following Kubernetes objects are included in this repository:

- Namespace
- PersistentVolume
- PersistentVolumeClaim
- StatefulSet
- Deployment
- Service

## Deployment Instructions

1. Create the namespace:

   ```sh
   kubectl apply -f manifests/namespace.yaml
