# VM-Management

## - This package is being used to configure all remote machines by ansible

- Configure multiple VMs is so painful, thanks to Ansible that make the configuration and the deployment as easy as possible.

- Remember to add hosts in file `inventory.ini` for configuring and deploying synchronously.

- To add new group and user from multiple instance, run the following command:

```
ansible-playbook playbooks/grant_permission_for_user_in_vm.yml
```

- To revoke a user from group of instance, please execute the command

```
ansible-playbook playbooks/revoke_user.yml -e "user_to_revoke=ansible"
```



- Thanks to vagrant for helping me provision vms in order to test.

