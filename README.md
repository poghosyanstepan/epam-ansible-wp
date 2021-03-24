# epam-ansible-wp
Install wordpress Ansible playbook
Instractions https://linuxconfig.org/ubuntu-20-04-wordpress-with-apache-installation
#1

## Աշխատանք 
cd /To/git/epam-ansible-wp

ansible -m ping all -i inventory/hosts

ansible-playbook -i ./inventory/hosts Install-wp.yml 
-vvvv --ask-vault-pass --ask-become-pass --limit webservers 

# Links
1. https://www.digitalocean.com/community/tutorials/how-to-use-ansible-to-install-and-set-up-wordpress-with-lamp-on-ubuntu-18-04-ru
2. https://www.infinitypp.com/ansible/install-wordpress-using-ansible-ubuntu-php7/
3. MariaDB - https://mariadb.com/kb/en/existing-ansible-modules-and-roles-for-mariadb/
4. community.mysql.mysql_user https://docs.ansible.com/ansible/latest/collections/community/mysql/mysql_user_module.html#examples
5. community.mysql.mysql_db - https://docs.ansible.com/ansible/latest/collections/community/mysql/mysql_db_module.html#examples
6. https://github.com/bertvv/ansible-role-mariadb/blob/master/tasks/root-password.yml
7. https://stackoverflow.com/questions/40050219/rootlocalhost-password-set-with-ansible-mysql-user-module-doesnt-work
