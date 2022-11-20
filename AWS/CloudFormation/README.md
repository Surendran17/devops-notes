# mini-network
repository is created to store code that will generate a mini-network in cloud formation

Resources Created : 
1. VPC
2. 3 private subnets in 3 AZs
3. 3 public subnets in 3 AZs
4. Route table
5. Security group for every Ec2(Jumpbox,App) and RDS instance
6. Nacl for public and private subnets.
7. Jumpbox Ec2 in private subnet and App Ec2 in private subnet. 
8. RDS instance in private subnet.

Stacks :
1. root-cloudformation  :  root stack
2. vpc-creation : Creates VPC,subnets,routes,route Table,gateway.
3. security-group-creation : Creates all the security groups for jumpbox,AppServer and RDS Instance.
4. nacl-creation : Creates nacl for public and private subnets.
5. ec2-creation : Creates jumpbox and AppServer instances
6. rds-creation: Creates rds instance.
