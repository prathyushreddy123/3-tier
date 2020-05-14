# 3-tier
Terraform is suitalbe for provisioning and created the template from scratch with the help of terraform documentation and other articles from medium. This is a basic 3-tier production grade infrasturcture I created with terraform as a part of practice. 
Below are the steps and aws services to get created from the template.
1. AWS VPC
2. subnets (for web application, backend application and database tier). Two subnets have been alloted for each tier and one in each AZ.
Here web will belongs to the public subnet and app and database to private subnet.
3. IGW
4. Route tables for public subnet
5. Associated the created route tables to the public subnets.
6. Route tables for private subnet
7. Associated the created route tables to the private subnets.
8. Public subnet to associate NAT gateway and bastion host.
9. NAT gateway
10. Associated NAT gateway to the public subnet (not to the web app in public subnet).
11. Create RDS instance
12. Created instance in web layer
13. Attached a security group to the web layer.
14. Load balancer in the web layer.
15. Created listeners and target group with the load balancer.

