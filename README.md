# Terraform for node sample app
This terraform code will generate an instance, in AWS in the region eu-west-1, using an AMI (which already has the app and dependencies installed onto it). It will create a VPC, internet gateway, route table (with association), subnets and security groups.

# Start up an instance
Run the following code in the command line
`terraform init`
`terraform plan`
`terraform apply`

# Load app
Place the ip address generated from the instance and give it port 3000 in the browser
xxx.xxx.xxx.xxx:3000

# If port 3000 isn't running
Using the key_name specified and ip generated from the instance enter the machine by running the following code into the command line:
`ssh -i ~/.ssh/key_name ubuntu@xxx.xxx.xxx.xxx`
`cd home/ubuntu/appjs/app`
`sudo npm install`
`sudo npm start`
