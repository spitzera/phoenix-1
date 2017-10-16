# Kubernetes 101 Challenge
In this chapter you will set up a Kubernetes cluster in Azure Container Services (ACS) and an Azure Container Registry (ACR) to store your images.

## 1. Create a Kubernetes cluster on Azure Container Services 
- Set up your Kuberenetes cluster using Azure Container Services.
> Need help? Check hints [here :blue_book:](hints/createk8scluster.md)!

The deployment will take some time (~20 min). 

## 1. Run single container app in your K8s cluster
> Need help? Check hints [here :blue_book:](hints/k8sSingle.md)!
- Run a public available application in a single container on your cluster. The image name is "nginx".
    - Use the "kubectl run" command
- Add a service to make your application accessible from the internet
    - Use the "kubectl expose" command and "kubectl edit YOURSERVICE" command.
- Start your webbrowser to view your application running in your cluster.

## 1. Kubernetes discovery
- Open the K8s portal for a graphical interface. Run `kubectl proxy`then open up a browser an navigate to http://localhost:8001/ui.

- Familiarize yourself with the following commands on commandline, eg.
```
kubectl get pods    // to display all pods
kubectl get svc     // to display all services
kubectl get deployments     // to display all deployments
kubectl delete pods/<podid> // to delete a specific pod

```
