# Engage-Coding-Challenge

# Description 
Provisioning of EC2 instance using ansible playbooks and cloudformation template as an input. I have included python code to check the health of the server, it also check if the service is up and its clock is not desynchronised by more than 1 second.

# Files

1. Webservice.yaml --> cloudformation template
2. Deploy_cloudform.yml --> playbook to create the cloudformation stack
3. Deploy_now.yml --> This playbook configure's the server to display the time.
4. Test_aws_ec2.yml --> This is a dynamic inventory file to be given as input to run the playbook -- deploy_now.yml
5. Main.py --> This is a python code to check the health of the service and give both the URL time and server time.

# Pre-Requisite
1. Need an ansible server hosted on linux with boto3 and botocore and configured to use python3
2. Ansible file configured to use the aws_ec2 plugin
3. Ansible file configured to use the access key specified to access the instance 
