# AWS deploy (Ansible EC2 module)

Deploy an instance on AWS EC2 service.

## Requirements

 - [x] pip
 - [x] virtualenv

## Settings

Edit vars in the playbook:
 - [x] key_name: rfolco-key
 - [x] aws_region: us-east-1
 - [x] ami_id: ami-26ebbc5c
 - [x] instance_type: t2.micro

## Usage

```
virtualenv .venv
source .venv/bin/activate
pip install ansible
pip install boto

export AWS_ACCESS_KEY_ID='MYKEYMYKEYMYKEYMYKEYMYKEY'
export AWS_SECRET_ACCESS_KEY='mysecretMYSECRETmysecretMYSECRET'

ansible-playbook -i inventory/hosts playbooks/aws-deploy.yml 

source .venv/bin/deactivate
```

## Reference

* (http://docs.ansible.com/ansible/ec2_module.html)
