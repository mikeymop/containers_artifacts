# Important commands

## AZ CLI

Gets kube creds from AZ portal
```
az aks get-credentials --resource-group myResourceGroup --name myAKSCluster
```

## Kubernetes

Apply a deployment spec to the cluster
```
kubectl apply -f <filename.yml>
```