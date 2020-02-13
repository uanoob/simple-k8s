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
# List running Services on local machine
    - kubectl get services
# Minikube Ip on local machine
    - minikube ip
## 192.168.99.100 (example)
# View running app in browser
     - <minikube ip>:<nodePort>
     - 192.168.99.100:31515
