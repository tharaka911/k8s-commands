
<!-- GETTING STARTED -->
## nawwa pack of k8s ammos for simple k8s cluster creating


### kubectl apply commands in order

```sh
kubectl apply -f mongo-secret.yaml
 ```
```sh
kubectl apply -f mongo.yaml
```
```sh
kubectl apply -f mongo.yaml
```
```sh
kubectl apply -f mongo-configmap.yaml 
```
```sh
kubectl apply -f mongo-express.yaml
```

### kubectl get commands
```sh
kubectl get pod
```
```sh
kubectl get pod --watch
```
```sh
kubectl get pod -o wide
```
```sh
kubectl get service
```
```sh
kubectl get secret
```
```sh
kubectl get all | grep mongodb
```
### kubectl debugging commands
```sh
kubectl describe pod mongodb-deployment-xxxxxx
```
```sh
kubectl describe service mongodb-service
```
```sh
kubectl logs mongo-express-xxxxxx
```
### kubectl debugging commands
```sh
minikube service mongo-express-service
```
 





  
