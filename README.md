# mysql
Ansible role to install mysql

Config as follows:

mysql_version: 5.5
mysql_root_password: change_me

#Optionally add databases as a list
mysql_databases:
    - db1
    - db2

#Optionally add users as a dictionary
mysql_users:
    user:
      name: change_me
      password: change_me
      privileges: *.*:ALL,GRANT
