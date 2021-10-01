# AWS-SAA-Cantril
>These are my notes from Cantril's course SAA(CO2)

- [1.1 Cloud Services]
- [1.2 EC2]
- [1.3 S3]
- [1.4 Route 53]


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

## 1.2 EC2(Elastic Cloud Compute)
- IAAS
- Private by Default
- provides access to virtual machines know as instances 
- only have no charges when terminated

**AMI (Amazon Machine Image)**
- server image used to create virtual machines

## 1.3 Simple Storage Service(S3)
- object storage object size rang 0 to 5TB
- object stored in bucket
- **bucket name has to be globally unique**

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
## 1.4 Route 53
- allows you to register domains
- globally resilient and global service
