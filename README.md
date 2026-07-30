For non cluster start: <br>
ansible-playbook -i inventory/hosts.yml playbook.yml <br>
<br>
For start with cluster: <br>
ansible-playbook -i inventory/hosts.yml playbook.yml -e "rabbitmq_mode=cluster" <br>
<br>
For cluster only: <br>
ansible-playbook -i inventory/hosts.yml playbook.yml --tags join_cluster -e "rabbitmq_mode=cluster"
