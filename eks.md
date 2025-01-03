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
