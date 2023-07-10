# EC2

EC2 - Elastic Compute Cloud - Infrastructure as a Service

consists capability of :

- renting virtual machines
- storing data on virtual drives
- distributing load across machines
- scaling the services using an auto scaling group

EC2 sizing & config options:

- OS
- Compute power and cores
- RAM
- Storage space (ebs & efs)
- Network card
- Firewall rules - security group

Userdata - set of commands that are run on the first launch

AWS naming convenction

m5.2xlarge

m: instance class
5: generation (AWS imrpoves these over time)
2xlarge: size within instance class

### EC2 Instance Types

1. General Purpose:

- great for diverse workloads, webservers / code repos
- balance between compute, memory & networking
- t2.micro is general purpose

2. Compute Optimized:

- good for compute intensive tasks i.e. batch processing workloads, gaming servers, scientific modeling and machine learning, high performance computing, high performance web servers, media transcoding
- start with C

3. Memory optimized:

- fast performance for workloads processing large data sets
- high performance databases, dist web scale cache stores, in-memory optimized for BI
- Applications performing processing of big unstructures data

### Security Groups

- can be attached to mulitple instances
- locaked down to a region / vpc
- sc groups live outside the ec2 - blocked traffic can't be seen
- if application is not acessible (time out), it's a security group issue
- All inbound traffic is blocked by default
- All outbound traffic is authorised by default

NOTE: separate security group for SSH access
