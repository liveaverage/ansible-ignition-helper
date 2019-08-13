# ansible-ignition-helper

Provides quick and dirty method to prepare OpenShift 4 DNS, Ignition Templates, and supporting VMware virtual machines for baremetal or vSphere UPI deployments

# Usage

1. Update cluster variables defined in each file, as applicable, in the `vars` directory
2. Update templates as needed in the `templates` directory
3. Make certain appropriate env variables are set for CloudFlare DNS and/or VMware environment management
4. Execute the playbook(s):

```
ansible-playbook -i localhost, prep_ocp_v4_dns.yml
ansible-playbook -i localhost, prep_ocp_v4_ignition.yml
```


