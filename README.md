# Use Case #

Helps automate creation of dhcpd.conf file for ZTP use-cases

# group_vars/all.yaml #

- Fill up this file with the dhcp parameters for individual hosts
- host_subnet is the subnet range for the ZTP hosts
- server_subnet is the subnet range of the ZTP/CVP server. This is required for the DHCP service to start.

## execution of the playbook ##  

```
ansible-playbook -i hosts dhcp-conf-creator.yaml
```

This should create dhcpd.conf file in the config directory
