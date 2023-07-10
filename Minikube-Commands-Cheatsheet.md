# Minikube Commands Cheatsheet

## Cluster Management

### `minikube start`
Starts a local Kubernetes cluster using Minikube.

### `minikube stop`
Stops the running Minikube cluster.

### `minikube status`
Displays the status of the Minikube cluster.

### `minikube delete`
Deletes the Minikube cluster.

### `minikube dashboard`
Opens the Kubernetes dashboard in a web browser.

## Resource Management

### `kubectl get nodes`
Lists the nodes in the Minikube cluster.

### `kubectl get pods`
Lists the pods running in the Minikube cluster.

### `kubectl get services`
Lists the services running in the Minikube cluster.

### `kubectl get deployments`
Lists the deployments running in the Minikube cluster.

## Deployment Management

### `kubectl create deployment [deployment-name] --image=[image-name]`
Creates a deployment in the Minikube cluster using the specified image.

### `kubectl expose deployment [deployment-name] --type=NodePort --port=[port]`
Exposes a deployment as a service in the Minikube cluster on a specified port.

### `kubectl scale deployment [deployment-name] --replicas=[replica-count]`
Scales a deployment to the specified number of replicas.

### `kubectl delete deployment [deployment-name]`
Deletes a deployment from the Minikube cluster.

## Service Management

### `minikube service [service-name]`
Opens a service in the Minikube cluster in a web browser.

## Logging and Debugging

### `kubectl logs [pod-name]`
Displays the logs of a specific pod in the Minikube cluster.

### `kubectl exec -it [pod-name] -- [command]`
Executes a command within a specific pod in the Minikube cluster.

## Port Forwarding

### `kubectl port-forward [pod-name] [local-port]:[remote-port]`
Forwards traffic from a local port to a specific pod in the Minikube cluster.

## Configuration and Add-ons

### `minikube config set [property-name] [property-value]`
Sets a configuration property for Minikube.

### `minikube addons list`
Lists the available add-ons for Minikube.

### `minikube addons enable [addon-name]`
Enables a specific add-on in the Minikube cluster.

### `minikube addons disable [addon-name]`
