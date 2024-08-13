** K8S CLuster **

** Workstation **

1. Create an EC2 instance for workstation.
2. Workstation needs to have some packages, which i mentioned below 
   Docker
   kubectl
   Eksctl
   Kubens 
```
sudo sh installation.sh
```
3. here, i'm using default VPC with default security group.
4. Configure AWS 
    accesskey
    secretkey
    workstation should have access to connect AWS to provision EKS Cluster.
```
aws configure
```


