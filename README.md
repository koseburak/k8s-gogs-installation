# cloud-native-gogs
gogs installation on docker, kubernetes and openshift

### gogs deployment on kubernetes
create persistent volume and claim
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-gogs/master/k8s/gogs-persistentvolume.yaml
```
create node port service
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-gogs/master/k8s/gogs-service.yaml
```
create config map
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-gogs/master/k8s/gogs-configmap.yaml
```
create deployment
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-gogs/master/k8s/gogs-deployment.yaml
```
