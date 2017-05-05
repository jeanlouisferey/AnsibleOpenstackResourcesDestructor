Ansible playbook for cloud tenant destruction (complete resource deletion)

## BE CAREFULL - This playbook is dangerous !##

===============================================

Today this playbook destroys automatically :
- instances
- volumes
- ports
- routers
- networks
- security groups
- keypairs
- floating IPs

It does not destroy (today):
- FWAAS
- LBAAS

===============================================

How to call playbook:

```ansible-playbook destructor.yml -e "@cloudresourcefile.yml"```

You will find a sample of cloud resource file in cloudresourcefile.yml.sample

Be carreful, you have to fill every variables with the good value !
