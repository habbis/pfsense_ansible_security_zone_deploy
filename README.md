# pfsense ansible security zone setup


The playbook setup mystandard pfsense security zone that is  vlan + interface + firewall rules = security zone.

Some tips think about your network standard i use `10.0.0.0/24` for a standard network and for home/guest `192.168.0.0/24` and tird number ip the ip address is the vlan number so with `10.0.194.1` the number 194 is the vlan then automation is easier.


To install collection.

```
ansible-galaxy collection install pfsensible.core

```

Here is the link to [modules](https://github.com/opoplawski/ansible-pfsense)
