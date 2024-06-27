
# deploy an eks cluster
eksctl create cluster --name universe-cluster --region us-east-1 --nodegroup-name universe-nodes --node-type t2.medium --nodes 3 --nodes-min 1 --nodes-max 4 --managed
aws eks update-kubeconfig --region us-east-2 --name universe
