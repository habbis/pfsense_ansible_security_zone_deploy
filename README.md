# pfsense ansible security zone setup



The playbook setup mystandard pfsense security zone and its  vlan + interface + firewall rules = security zone.




Some tips think about your network standard i use `10.0.0.0/24` for a standard network and for home/guest `192.168.0.0/24` and tird number ip the ip address is the vlan number so with `10.0.194.1` the number 194 is vlan and automation is easier.

Another tip is to use alias for your firewall rules so its easier to add network to existing or future network/ipaddr to a rule. In the deploy and alias playbook i use dns_servers as an alias for a ip range.


The RFC_1918 alias is made for the standard block rule and it blocks all those networks in that standard.

```
10.0.0.0/8
172.16.0.0/12
192.168.0.0/16
```




To install collection.

```
ansible-galaxy collection install pfsensible.core

```

Here is the link to [modules](https://github.com/opoplawski/ansible-pfsense)
