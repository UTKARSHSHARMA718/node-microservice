# Kubernetes commands

### for creating a POD in kubernetes
- kubectl apply -f .\posts.yml

### for executing a given command inside a running pod
- kubectl exec -it [pod_name] [cmd]

### Print out logs from the given pod
- kubectl logs [pod_name]

### for deleting the given pod
- kubectl delete pod [pod_name]

### Tells kubernetes to process the config
- kubectl apply -f [config file name]

### Print out some information about the running pod
- kubectl decribe pod [pod_name]

### setup an alias -----------------------------------------------
- Set-Alias -Name k -Value kubectl

<!-- ------------------------------------------------ -->
# Deployments commands

### List all the running deployments
- kubectl get deployments

### Print out details about specific deployments
- kubectl describe deployments [depl name]

### Create a deployments out of a config file
- kubectl apply -f [config file name]

### Delete a deployments
- kubectl delete deployment [depl_name]

### restart the deployment (to get start the pods with latest images available)
- kubectl rollout restart deployment [delp_name]

noose
knit

# Skaffold

### To start skaffold
- skaffold dev
- (Make sure you are using 'nodemon' in node applications for re-starting the app once the skaffold update the changes file into the project directory)