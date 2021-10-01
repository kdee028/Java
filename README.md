# AWS-SAA-Cantril
>These are my notes from Cantril's course SAA(CO2)

- [1.1 Cloud Services](#11-cloud-services)
- [1.2 EC2](#12-ec2)
- [1.3 S3](#13-s3)
- [1.4 Route53](#14-route53) 



## 1.1 Cloud Services 
1.	Infrastructure as a Service -vendor manages, pay per sec or min 
2.	Software as a Service-you consume Ex: Netflix
3.	Platform as a Service (PaaS) you manage app and data, vendor mange everything else
4.	On-premises-individual manages all components 
5.	Data center hosting-place equipment, you pat for facility

- Public Cloud=1 AWS public cloud
- Private Cloud=using on-premises real cloud
- Multi-Cloud=more than 1 public cloud
- Hybrid Cloud=using public and private in on environment 
  - this is **not** public and legacy on premises 

- **Region**-area with full AWS deployment
- **edge locations**- local distribution points 

**VPC (Virtual Private Cloud)**-virtual network inside AWS
- one default VPC per region can have many customs 
- do not use default VPC
- one subnet in each AZ

## 1.2 EC2
- IAAS
- Private by Default
- provides access to virtual machines know as instances 
- only have no charges when terminated

**AMI (Amazon Machine Image)**
- server image used to create virtual machines

## 1.3 S3
- object storage object size rang 0 to 5TB
- object stored in bucket
- **bucket name has to be globally unique**

Identity
- Controlling high mix of different resources.
- Not every service supports resource policies.
- Want to manage permissions all in one place, use IAM.
- Must have access to all accounts accessing the information.

Bucket
- Managing permissions on a specific product.
- If you need anonymous or cross account access.
- **enabled bucket can never be switch backed to disables**

Versioning
- allow bucket to satore multiple versions of objects 
- objects aren't deleted deletion markers are put in place to hide objects 
- can ony be suspended

MFADelete 
- required to delete versions
- required to change bucket versioning state

Single PUT Upload 
- single data stream to s3
- stream fails =upload fails

Multipart upload 
- breaking data into parts 
- min data size of 100Mb


















**Cloud Formation (infrastructure as a Code)**
- uses a template to create AWS Infrastructure 
- uses YAML or JSON
- only required is the resource section
- Description must directly follow template format version
  - Cloud Watch
    - Monitoring of Metrics
- CloudTrail: who accessed and when they accessed 

**Domain Name Sever (DNS)**
- 13 DNS root servers
- EX: when connecting to website (host to IP)
- discovery service-translate machine into human
- A-host to IPV4
- AAAA-host name to ipv6
-	CNAME-host to host cannot point to IP
- TXT-to prove domain ownership
-	MX-how emails are sent 
-	NS- delegates control of .org to the .org registry

**High Availability**-system that maximizes uptime

**Fault tolerant**- system that allows failure and can operate without interruptions

## 1.4 Route53
- allows you to register domains (Domain Name System Service)
- globally resilient and global service


