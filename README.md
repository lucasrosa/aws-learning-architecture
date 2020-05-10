## Requirements


### Load Balancer
* Use ALB - Application Load Balancer
* Load Balancer must be private

### CloudFormation
* Everything must be done as IAC
* Make use of Parameters
* Changes done through change sets
* Important information should be on Output (dns)

### CloudWatch
* Detailed Monitoring enabled
* Send notifications to email
    * CPU reaches 90%
    * Disk reaches 80%

### CloudTrail
* New EC2 Instance created

### EC2
* Each instance in the auto-scaling group must be in a different availability zone
* Responses from the webservers must include their private IP (to see if load balancer is working)

### VPC
* Database and application instances must be in a private subnet
* Flow logs enabled

### S3
* Make use of all S3 storage classes  

### CloudFront 
* Distribution for S3 content

### Route53
* Application should use a real domain

### SNS

### IAM
* Minimum privilege
* Groups
    * Engineering
    * Auditing
    * Monitoring

### VPN
* Site to site