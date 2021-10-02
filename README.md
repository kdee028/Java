# AWS-SAA-Cantril
>These are my notes from Cantril's course SAA(CO2)

- [1.1 Availability Zones](#11-availability-zones)
- [1.2 IAM](#12-iam)
- [1.3 AWS ACCESS](#13-aws-access)
- [1.4 AWS KMS](#14-aws-kms)
- [1.5 AWS Shield](#15-aws-shield)

## 1.1 Availability Zones
Region
- physical locations with clusters of data centers

Availability Zones 
- discrete data center 
- AZs in a region are usually 3, min is 2 and max is 6

## 1.2 IAM
Identity  and Access management
- users:mapped to physical user 
- groups:can have one or more users

Least Principle Priviledge

Policies: JSon documents that **allow or deny** permissions

IAM Permission Boundaries
- defines max allowed permissions

AWS Certificate Manager(ACM)
- manages SSl/TLS certificates
**SSL and TLS enable traffic between the client and the Load Balancer 

IAM Certficate Store 
- where 3rd party SSL/TCL certs are uploaded
## 1.3 AWS ACCESS
- AWS Management Console
- AWS CLI or SDK
- AWS CLoudshell:CLI tool from browser

**NON-IAM Users**
- STS(Security Token Service): Up to 1hr of access

## 1.4 AWS KMS
Key Management Service 

## 1.5 AWS Shield
Disributed Denial of Service(DDoS) protection service 
- protects up to 97% of DDoS attacks 

AWS Shield Standard  is automatic and free

AWS WAF(Web Application FIrewall)
- protects weications against web exploits 
- prootects Layer 7(HTTP)

AWS Firewall Manager
- to centralloy configure and manage AWS Shield & WAF rules
## 1.6 EC2(Elastic Compute Cloud)
virtual machine on the cloud 
- IaaS
**EC2 Launch Types**
- On demand: pay as you use 
- Reserved: for 1 or 3 years
- Scheduled Reserved Instances: reserved capacity that is scheduled
- Spot Instances: up to 90% discount 
   - spot block:
   - Spot fleet: spot and on-demand instances 
 - Dedicated instance: instance on dedicated hardware
 - Dedicated Host- instance run on dedicated server
EC2 Hibernate: save contents of instance memory ram


Elastic Network Interface(ENI)
- provide internet to EC2 instance 
- virtual network card that you attach an EC2 instance to

EC2 placement Types 
-  cluster: Low latency, high network, HPC(High performance computing)
-  spread: high availability critical apps
-  partition:distributed apps like Cassandra 

AMI amazon machine image 
- can create an AMI from EC2 instance 

Load balancers: direct internet traffic to and from EC2 instances 
Elastic Load Balancers 
- Application Load Balancer	HTTP, HTTPS, WebSocket
- Network Load Balancer	TCP, UDP, TLS
- Gateway Load Balancer	Thirdparty appliances
- Classic Load Balancer (old)	HTTP, HTTPS, TCP 

