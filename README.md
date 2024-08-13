**K8S CLuster**

**Workstation**

1. Create an EC2 instance for workstation.
2. Workstation needs to have some packages, which i mentioned below 
   Docker
   kubectl
   Eksctl
   Kubens 
```
sudo sh installation.sh
```
3. Here, i'm using default VPC with default security group.
4. Configure AWS, workstation should have access to connect AWS to provision EKS Cluster.
```
aws configure
```
**EKS**

EKS is AWS Kubernetes service. EKS is the master node completely managed by AWS.

- we are going to use EKS managed node group, we need to worry about installation, underlying OS, etc
- create one key-pair and import public key into AWS.
```
eksctl create cluster -f cluster.yaml
``` 


