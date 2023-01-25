# Important commands

## AZ CLI

Gets kube creds from AZ portal
```
az aks get-credentials --resource-group myResourceGroup --name myAKSCluster
```

Connect Kubernetes instance to the AKS container registry
```
az aks update -n testAKSCluster -g teamResources --attach-acr registryidq6940
```

## Kubernetes

Apply a deployment spec to the cluster
```
kubectl apply -f <filename.yml>
```

Debugging: Execute a command in an already deployed container from within the Kubes network
```
kubectl exec --stdin --tty poi-deployment-58978fb684-vftgg -- curl -i -X GET 'http://localhost:80/api/poi/healthcheck'
```