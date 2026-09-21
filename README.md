# k8s-deployment-service

A minimal Kubernetes demo showing how to deploy an application using a Deployment and expose it using a Service.

## Files

- deployment.yaml — defines a Deployment with 2 replicas of an NGINX container
- service.yaml — exposes the Deployment using a NodePort Service

## Apply

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

## Check

kubectl get pods
kubectl get svc

Access the app:

http://<node-ip>:30080

