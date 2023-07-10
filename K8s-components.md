# K8s components

1. **Pod**: A pod is the smallest deployable unit in Kubernetes. It represents a single instance of a running process within the cluster. Typically, a pod contains one or more containers that are tightly coupled and share the same resources.

2. **ReplicaSet**: A ReplicaSet ensures that a specified number of pod replicas are running at all times. It helps maintain the desired state by creating or deleting pod replicas as needed, based on the defined replica count.

3. **Deployment**: A Deployment is a higher-level abstraction that manages the lifecycle of ReplicaSets. It allows you to declaratively define and manage the desired state of your application. Deployments handle updates, rollbacks, and scaling of your application by creating or modifying underlying ReplicaSets.

4. **Service**: A Service provides network connectivity to a set of pods. It abstracts away the dynamic IP addresses of the pods and provides a stable endpoint for accessing them. Services enable load balancing, service discovery, and internal communication between pods.

5. **Ingress**: An Ingress is an API object that manages external access to services within a cluster. It acts as a gateway, routing incoming requests to the appropriate services based on rules and configurations. Ingress can provide features like SSL termination, virtual hosting, and path-based routing.

6. **ConfigMap**: A ConfigMap holds configuration data as key-value pairs that can be consumed by pods. It allows you to separate configuration from your application code and provides a way to modify configuration without redeploying the entire application.

7. **Secret**: Secrets store sensitive information like passwords, API tokens, or certificates. They are similar to ConfigMaps but are base64 encoded and provide additional security features. Secrets are mounted as files or environment variables in pods.

8. **Namespace**: A Namespace is a logical boundary within a Kubernetes cluster. It allows you to create isolated environments and organize resources. It helps avoid naming conflicts and provides resource quota and access control for different teams or projects.

9. **Node**: A Node is a physical or virtual machine within a Kubernetes cluster. It acts as a worker that runs pods and other cluster components. Nodes are managed by the cluster's control plane and are responsible for executing the requested workloads.

10. **Cluster**: A Cluster is a set of physical or virtual machines (nodes) that collectively run containerized applications. It consists of a control plane (master) and multiple worker nodes. The control plane manages and orchestrates the cluster, while the worker nodes execute the workloads.
