CrashLoopBackOff:

Cause: error in image. 
Fix: fixed and updated image. delete and reapplied deployment

kubectl delete deployment planet-facts-deployment

docker inspect 533266979424.dkr.ecr.us-east-1.amazonaws.com/planet-facts-service:latest

kubectl logs planet-facts-deployment-bcb99ffcc-btz54

kubectl apply -f planet-facts-deployment.yaml
