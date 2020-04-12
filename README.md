###  Ansible role to Install LAMP stack on Linux (Amazone linux, etc)

This role can be used to install a fully featured LAMP stack on Amazon Linux. Tihs can be used to deply a full WordPress installation or any CMS/Application that works over a LAMP stack.

#### Fetaures

  - Fully confgurable and compatible with AWS
  - Flexible and feature rich with easy customization of roles
  - Can be modified to support additional modules
  - Can be used to create a standalone LAMP stack or deploy applications over the current LAMP stack

#### For Customization
> Edit roles/default/main.yml 
- mysql_root: This variable defines the root password ofthe MySQL database
- mysql_user: This variable defines the additional database user 
- mysql_password: This variable defines the additional MySQL database password
- mysql_database: This variable defines the additional MySQL database name
> Additional user will have full privilege on the mysql_database 

#### How to change DB settings

```
$ cat var/main.yml
---
mysql_root: mysqlroot123
mysql_user: mysqluser123
mysql_password: mysqlpassword
mysql_database: mysqldb
domain: www.praveen.com
```
