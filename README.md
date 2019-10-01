# Ansible Patch

# How to use it
## to patch a list of package:
ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t package_list -u root -k

## to patch a adv:
ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t adv -u root -k

## to patch a cve
ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t cve -u root -k

## to patch a whole environment
ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t date -u root -k

## to reboot
ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t reboot_no_dbs -u root -k

ansible-playbook -i ../ansiblefest/inventory_service_ansible patch_all.yml -l prd -t reboot_mysql -u root -k