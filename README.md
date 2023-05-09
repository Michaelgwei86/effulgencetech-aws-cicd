# effulgencetech-aws-cicd-project
Docker, Buildspec, Infra, App
# Infrastructure details
>>Consists of a VPC -----> 10.0.0.0/16
>> Consists of Two public subnets
    Public subnet 1 ------> 10.0.0.0/24
    Public subnet 2 ------> 10.0.1.0/24
>> Consists of Two private subnets
    Private subnet 1 -----> 10.0.2.0/24
    Private subnet 2 -----> 10.0.3.0/24
>> An Internet Gateway to the the VPC
>> A public route point to 0.0.0.0/0 attached to the Internet Gateway
>> Route table associations
>> NAT Gateway and NAT Gateway attachments
>> Application load balancer (ALB) components
    > ALB security group
    > ALB attachment to IGW
    > Target group
>> ECS Cluster
    > Cluster security group

# IAM Service Roles
>> Autoscaling Role
>> EC2 Role
>> EC2RoleInstanceProfile
>> ECS Role

# Fargate Service 

Deploy an ECS service on  AWS Fargate
>> Service name ----> aws-cicd-demo-service
>> Setup default Image from Dockerhub