# simple-k8s
Docker and Kubernetes
# Prepare environment on local machine
    - Install Kubectl
    - Install Virtualbox
    - Install Minikube
# Start minikube on local machine
    - minikube start
# Stop minikube on local machine
    - minikube stop
# Status minikube on local machine
    - minikube status
# Cluster info on local machine
    - kubectl cluster-info
# Change the current config of cluster
    - kubectl apply -f <filename>
    - kubectl apply -f client-pod.yaml
    - kubectl apply -f client-node-port.yaml
# List running Pods on local machine
     - kubectl get pods
# List running Pods on local machine with ip inside virtual machine
     - kubectl get pods -o wide
# List running Services on local machine
    - kubectl get services
# List running Deployments on local machine
    - kubectl get deployments
# Get detailed info about object
     - kubectl describe <object type> <object name>
     - kubectl describe pod client-pod
     - kubectl describe deployment client-deployment
     - kubectl describe service client-node-port
# Delete a running object
     - kubectl delete -f <config file>
     - kubectl delete -f client-pod.yaml
     - kubectl delete -f client-node-port.yaml
# Minikube Ip on local machine
    - minikube ip
## 192.168.99.100 (example)
# View running app in browser
     - <minikube ip>:<nodePort>
     - 192.168.99.100:31515
