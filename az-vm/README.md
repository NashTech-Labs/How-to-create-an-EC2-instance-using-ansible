# Description

This template is based on the ansible script and use to create an EC2 Instance in your aws account.
 
# Prerequisites:

* AWS credentials (Access key or Secret key)
* And the pem file.
* Install boto and boto3 in your local machine.
* Install ansible(latest version).

After fullfill the Prerequisites you can create your ec2 instance using this command :
 
ansible-playbook start.yml

This template create an ec2 instance(linux) in your aws account.
You can change your instance type, ami-id and regions in the vars file according to your need.

Note:
The credentials file is used to store the aws credentials (access key and the secret key).
and encrypt your credentials using ansible-vault command for the privacy.
* ansible-vault encrypt credentials # for the encrypt the file.
* ansible-vault decrypt credentials # for the decrypt the file.

After the encypt your aws credentials use this command to run the ansible playbook:

ansible-playbook start.yml --ask-vault-pass