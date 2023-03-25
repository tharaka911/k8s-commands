
<!-- GETTING STARTED -->
## nawwa pack of k8s ammos for simple k8s cluster creating

### create minikube cluster


```sh
minikube start 

kubectl get nodes

minikube status

kubectl version
```

### delete cluster and restart in debug mode
```sh
minikube delete

minikube start 

minikube status
```


### kubectl commands

```sh
kubectl get nodes

kubectl get pod

kubectl get services

kubectl create deployment nginx-depl --image=nginx

kubectl get deployment

kubectl get replicaset

kubectl edit deployment nginx-depl
```


### debugging
```sh
kubectl logs {pod-name}

kubectl exec -it {pod-name} -- bin/bash
```

### create mongo deployment
```sh
kubectl create deployment mongo-depl --image=mongo

kubectl logs mongo-depl-{pod-name}

kubectl describe pod mongo-depl-{pod-name}
```

### delete deplyoment
```sh
kubectl delete deployment mongo-depl

kubectl delete deployment nginx-depl
```

### create or edit config file
```sh
vim nginx-deployment.yaml

kubectl apply -f nginx-deployment.yaml

kubectl get pod

kubectl get deployment
```

### delete with config
```sh
kubectl delete -f nginx-deployment.yaml
```

### Metrics
kubectl top The kubectl top command returns current CPU and memory usage for a cluster’s pods or nodes, or for a particular pod or node if specified.

### kubectl apply commands in order

```sh
kubectl apply -f mongo-secret.yaml

kubectl apply -f mongo.yaml

kubectl apply -f mongo.yaml

kubectl apply -f mongo-configmap.yaml 

kubectl apply -f mongo-express.yaml
```

### kubectl get commands
```sh
kubectl get pod

kubectl get pod --watch

kubectl get pod -o wide

kubectl get service

kubectl get secret

kubectl get all | grep mongodb
```
### kubectl debugging commands
```sh
kubectl describe pod mongodb-deployment-xxxxxx

kubectl describe service mongodb-service

kubectl logs mongo-express-xxxxxx
```
### kubectl debugging commands
```sh
minikube service mongo-express-service
```

### kubectl making and changing the workplace

```sh
kubectl create namespace my-namespace

kubectl get namespaces

kubectl config set-context --current --namespace=my-namespace

kubectl get pods
```





  
