For non cluster start:
ansible-playbook -i inventory/hosts.yml playbook.yml
For start with cluster:
ansible-playbook -i inventory/hosts.yml playbook.yml -e "rabbitmq_mode=cluster"
For cluster only:
ansible-playbook -i inventory/hosts.yml playbook.yml --tags join_cluster -e "rabbitmq_mode=cluster"
