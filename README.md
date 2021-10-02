# AWS-SAA-Cantril
>These are my notes from Cantril's course SAA(CO2)

- [1.1 Availability Zones](#11-availability-zones)
- [1.2 IAM](#12-iam)
- [1.3 AWS ACCESS](#13-aws-access)
- [1.4 AWS KMS](#14-aws-kms)


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

##1.5 AWS Shield
Disributed Denial of Service(DDoS) protection



