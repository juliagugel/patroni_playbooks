# patroni_playbooks
The unbreakable, scalable elephant - playbooks 

This contains all the playbooks and templates I ran during my presentation at the pgconf 2019 in Milan.

In case you want to rerun the playbooks. You need 4 VMs for the patroni cluster (+1 for ansible):

1.  Run the playbook under "patroni" to install a 3 node patroni cluster.
2.  Run the playbook under "patroni_add" to install a 4th node.
3.  Run the playbook under "etcd_change" to add the 4th node to the existing cluster
4.  Run the playbook under "patroni_remove" to remove the 3rd node from the existing cluster

This playbooks are not perfect. Especially when adding/removing a node to/from an existing cluster. But they work ;-)

Please keep in mind that this playbooks install the DMK of dbi services as well. As this tool is only for our customers, I removed the files. You need to adjust the playbooks according to this.
