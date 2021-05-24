Create 
-> a VPC

-> 3 private subnets

-> One NAT Gateway

-> One route table with (aws_nat_gateway + 0.0.0.0/0) as a route & associate each private subnet with it

-> 3 public subnets

-> One Internet gateway

-> One route table with (aws_internet_gateway + 0.0.0.0/0) as a route & associate each public subnet with it

Launch an EC2 instance in the subnet main-public-1.
The instance must have access to the internet. All thanks to the internet gateway