create a cloudformation template that launches EC2 instances and sets up an Apache web sever within a vpc. 
The template should also create two subnets within the VPC, one for public-facing resources and one for private resources. 
The EC2 instances should be placed in the private subnet and the Apache web server should be accessible from the internet through a public subnet. 

Guidelines: 
 The VPC should have CIDR block of 10.0.0.0/16 . 
 The public subnet should have a CIDR block pf 10.0.1.0/24 and the private subnet should have a CIDR block of 10.0.2.0.24 . 
 The EC2 instance should us an Amazon linux 2 AMI and should be t2.micro type.  The EC2 instances should be accessible through SSH using an existing key pair.  
 The Apache web server should be installed on the EC2 instances and should display a default "Welcome to Apache"  page when accesed from a web browser. 
 The clodformation template should include the creation of all necessary  security groups, network interfaces and routing tables. 
 The cloudformation template should be written in YAML. 
 The 10 EC2 instances should be created in an Auto Scaling Group and be behind a Load Balancer to handle incoming traffic
 
 
 
Note: In the above template, replace "myKeyPair" with the name of your existing key pair. Also make sure that the region in which you are creating the resources supports the Amazon Linux 2 AMI (ami-0c55b159cbfafe1f0).
