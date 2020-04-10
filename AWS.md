### General
See [Regions, Availability Zones, and Local Zones](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
* AWS Cloud spans 55 AVs within 18 geographic regions

## Services
See [AWS Compute services](https://aws.amazon.com/products/compute/)
* VMs: __EC2__, __Lightsail__ (like EC2-lite)
* Serverless: __Lambda__ (no servers, just runs instances of code [i.e. realtime image-processing] in non-contiguous periods of time)
* Edge Computing (IOT): __Outpost__ (runs AWS services/APIs locally), [Local Zones (use AWS infrastructure in end-user's locality for use cases needing ultra low-latency)](https://aws.amazon.com/about-aws/global-infrastructure/localzones/?c=cp&sec=srv)
### Typical Architecture
1. Traffic from internet hits an __Elastic Load Balancer (ELB)__
2. __ELB__ distributes traffic to __EC2__ instances
3. Amazon Simple Storage Service (__S3__)
4. __DynamoDB__ Relational Database Service (RDS)

## VPC
### VPC with a Single Public Subnet
* Region, Availability Zone
* IP Range: __IPv4 CIDR block__, ex: 10.10.0.0/16
* __Subnet IPv4 CIDR:__ 10.10.1.0/24 
    *see [Subnetwork](https://en.wikipedia.org/wiki/Subnetwork)
