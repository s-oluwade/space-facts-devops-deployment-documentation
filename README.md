# Space Facts Microservice Application

Space facts is a microservice web application for space facts. It was built in python with the Flask framework. It comprises of the following 5 microservices:
1. moon-service
2. planet-service
3. star-service
4. aggregator-service
5. client-service

Deployed in Kubernetes via an EKS cluster

# deploy an eks cluster
eksctl create cluster --name universe-cluster --region us-east-1 --nodegroup-name universe-nodes --node-type t2.medium --nodes 3 --nodes-min 1 --nodes-max 4 --managed
aws eks update-kubeconfig --region us-east-2 --name universe
