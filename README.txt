This file defines the services, service accounts, and deployments for the Bookinfo sample.

To apply all 4 Bookinfo services, their corresponding service accounts, and deployments:
kubectl apply -f bookinfo.yaml

Alternatively, you can deploy any resource separately:
kubectl apply -f bookinfo.yaml -l service=reviews # reviews Service
kubectl apply -f bookinfo.yaml -l account=reviews # reviews ServiceAccount
kubectl apply -f bookinfo.yaml -l app=reviews,version=v3 # reviews-v3 Deployment
