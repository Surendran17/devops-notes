The tightly coupled architecture running on one single instance is evolved into elastic architecture 
which helps us to scale the application in and out. 

1. Launch template is created and used to automate the build of ec2 and installing necessary softwares. 
2. Take backup of SQL running in EC2 instance. Create an RDS instance in necessary subnet and
    load the backup into RDS instance. Update config in EC2 to make wordpress use RDS instance.
3. Create EFS and use the EFS to store and use images or other content needed for the website. 
4. Create an ASG and ALB with necessary configurations. 

Now the application elastic and each layer works independently and can be scaled in or out as per requirement.
 