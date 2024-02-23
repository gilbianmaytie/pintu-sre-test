# Pintu SRE Test Case

1. This program is running using Golang and Node Js in 2 different folders
2. You can access image registry from docker hub and is available for public (https://hub.docker.com/repositories/gilbianmaytie)
3. You can run both services on the kubernetes cluster, you can use minikube to run this

## How to run and expose to local ports
 - kubectl apply -f deployment-go.yaml
 - kubectl apply -f service-go.yaml
 - kubectl apply -f deployment-node.yaml
 - kubectl apply -f service-node.yaml
 - kubectl port-forward service/simple-golang-app 8080:9090
 - kubectl port-forward service/simple-node-app 3000:9091


