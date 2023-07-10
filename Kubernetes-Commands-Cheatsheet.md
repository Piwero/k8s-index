# Kubernetes Commands Cheatsheet

## Cluster Management

### `kubectl cluster-info`
Displays the information about the Kubernetes cluster including the API server URL, cluster version, and the Kubernetes master.

### `kubectl get nodes`
Lists all the nodes in the cluster along with their status, including their names, roles, and conditions.

### `kubectl get pods`
Lists all the pods running in the cluster, displaying their names, statuses, and the nodes they are scheduled on.

### `kubectl describe node [node-name]`
Provides detailed information about a specific node, including its capacity, allocatable resources, and conditions.

### `kubectl describe pod [pod-name]`
Displays detailed information about a specific pod, including its status, events, and the containers running inside it.

### `kubectl top node`
Shows CPU and memory usage statistics for each node in the cluster.

### `kubectl top pod`
Displays CPU and memory usage statistics for each pod in the cluster.

## Deployment Management

### `kubectl get deployments`
Lists all the deployments in the cluster, including their names, replicas, and available replicas.

### `kubectl describe deployment [deployment-name]`
Provides detailed information about a specific deployment, including its replicas, strategy, and events.

### `kubectl scale deployment [deployment-name] --replicas=[new-replica-count]`
Scales a deployment by updating the number of replicas to the specified count.

### `kubectl rollout status deployment [deployment-name]`
Checks the status of a deployment rollout, showing if it is progressing or has completed.

### `kubectl rollout history deployment [deployment-name]`
Displays the revision history of a deployment, including the timestamps and changes made to each revision.

## Service Management

### `kubectl get services`
Lists all the services in the cluster, including their names, cluster IPs, and exposed ports.

### `kubectl describe service [service-name]`
Provides detailed information about a specific service, including its type, endpoints, and selectors.

### `kubectl expose deployment [deployment-name] --port=[port] --target-port=[target-port] --type=[service-type]`
Creates a new service to expose a deployment, specifying the ports and type of service.

### `kubectl delete service [service-name]`
Deletes a service by specifying its name.

## Logging and Debugging

### `kubectl logs [pod-name]`
Displays the logs of a specific pod, showing the output of its containers.

### `kubectl exec -it [pod-name] -- [command]`
Executes a command within a specific pod, allowing you to interact with its containers.

### `kubectl describe pod [pod-name]`
Provides detailed information about a specific pod, including its status, events, and containers.

### `kubectl get events`
Lists all the events in the cluster, including their timestamps, types, and related objects.

## Resource Management

### `kubectl describe resource [resource-type]`
Provides detailed information about a specific Kubernetes resource, including its properties and status.

### `kubectl get [resource-type]`
Lists all the resources of a specific type in the cluster, displaying their names and properties.

### `kubectl delete [resource-type] [resource-name]`
Deletes a specific resource by specifying its type and name.
