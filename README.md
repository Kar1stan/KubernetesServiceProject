# KubernetesServiceProject
***
Simple kubernetes deployment manifect creating LoadBalancer service with 2 containers.

## 💻 Pre-requisites

Before you use this project you need to have Docker installed in your computer,and also Minikube.

https://www.docker.com/products/docker-desktop/
https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download

### Git clone
This will clone the project:
```
$ git clone https://github.com/Kar1stan/KubernetesServiceProject.git
$ cd KubernetesServiceProject
```

## 🚀 Run the manifest: 
To run the deployment with service,open the terminal and run:
```
$ kubectl apply -f service-myweb-v1.yaml
```
To delete deployment with service,open the terminal and run:
```
$ kubectl delete service service-myweb-v1
```
To show details of the service,open the terminal and run:
```
$ kubectl describe service my-multi-pods-service
```
To see results in the browser,paste External IP of the LoadBalancer with port of the container:

Example - 10.109.141.45:80

* in Windows External IP is forever "pending" ,so use Cluster IP instead

