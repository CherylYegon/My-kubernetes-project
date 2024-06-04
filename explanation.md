# Explanation of Kubernetes Implementation

## Choice of Kubernetes Objects
For the application deployment, I chose to use a Deployment object because it provides a declarative update to applications. I used a StatefulSet for the database because it requires stable, unique network identifiers and persistent storage.

## Exposing Pods to Internet Traffic
I used a Service of type LoadBalancer to expose the application pods to external traffic. This provides an external IP address that forwards traffic to the application.

## Persistent Storage
I used PersistentVolume and PersistentVolumeClaim to provide persistent storage for the StatefulSet. This ensures that the database data persists even if the pods are deleted and recreated.

## Git Workflow
I used a feature-branch workflow, where each new feature or bug fix was developed on a separate branch. Once the feature was complete, it was merged into the main branch after review.

## Debugging Measures
I ensured the application was running correctly by checking the status of pods and services using kubectl commands and reviewing logs for errors.
