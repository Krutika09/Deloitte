## Installation of Docker
**AWS Ec2**
- Create an Ec2 Instance
- Select Linux AMI
- Select your key-pair
- Launch Instance & connect that instance.

**Installation of Docker**
**1. To install Docker**
```
yum install docker
```
**2. Start Docker**
```
systemctl start docker
```
**3. Pull Image from DockerHub**
```
 docker pull ubuntu:14.04
```
**View images**
```
docker images
```
![image](https://github.com/user-attachments/assets/239f363c-9988-499e-85d5-49fd4305541f)

**4. Run container from image.**
```
docker run -tid ubuntu:14.04
```
**View container**
```
docker ps
```
![image](https://github.com/user-attachments/assets/bdd8da16-6075-4ac5-bd24-9e0ab781f5a3)

**5. To view details of container**
```
docker inspect container-id
```
**Copy the ip of container**
```
 curl http://172.17.0.3
```
![image](https://github.com/user-attachments/assets/e5967374-8d53-4477-bbe5-7cbe0693a1e4)
