## To Create EKS cluster from command prompt(cmd)
**1. Go to your Command prompt and Configure AWS**
```
aws configure
```

![image](https://github.com/user-attachments/assets/2c6a75a5-717f-4fda-bc66-da1e5dcee682)

**2. Create Cluster**
```
eksctl create cluster --name newcluster
```
**It start creating your cluster.**
![image](https://github.com/user-attachments/assets/a9fc6e85-f806-4b65-ae1d-3af5b0063b1e)
**Your Cluster is successfully.**
![image](https://github.com/user-attachments/assets/3bebac50-ee54-4414-8411-1bad0fae4e22)

**3. View created cluster name.**
```
aws  eks  list-clusters
```
![image](https://github.com/user-attachments/assets/8fad06af-a70b-41b4-86fe-465ac97147c0)

**4. View your created Nodes**
```
kubectl get nodes
```
![image](https://github.com/user-attachments/assets/b16379b2-7b2d-4183-98dd-f8f623cb7ab7)

![image](https://github.com/user-attachments/assets/747d190a-b896-47f5-a014-9dd220584627)

![image](https://github.com/user-attachments/assets/911c57ba-4129-4172-a508-2338e0b61f10)

**5. Delete cluster**
```
eksctl delete cluster --name=newcluster
```
## Deployment

**1. To Create Deployment**
```
kubectl create deployment myweb --image=vimal13/apache-webserver-php
```
**2. View Deployment.**
```
kubectl get deplotment
```
![image](https://github.com/user-attachments/assets/3513453c-10e3-4c77-ad7d-6b81dd59f65c)

**3. Delete deployment**
```
kubectl delete deployment dep-name
```

## Replicas
**1. To create replicas**
```
kubectl scale deployment myweb --replicas=4
```

**2. To view replicas**
```
kubectl get pods
```
![image](https://github.com/user-attachments/assets/82d2c3c6-7cc5-4016-a85a-33ba4cf34658)


## Service - LoadBalancer
**1. Command to create LoadBalncer**
```
kubectl expose deployment myweb --type LoadBalancer --port 80 --target-port 80
```
**2. View LoadBalancer**
```
kubectl get svc/service
```
![image](https://github.com/user-attachments/assets/2d7e761c-2dea-4f0b-aedc-32f5cfca2c33)


![image](https://github.com/user-attachments/assets/d094f7dd-4979-4d1c-b84f-259dbbb864d7)

**If you hit external-ip then you see the page**

![image](https://github.com/user-attachments/assets/4386af37-778a-4297-8e08-8462daac3409)
