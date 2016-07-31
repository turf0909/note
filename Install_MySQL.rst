2016.07.30 
==========

**Install MySQL 5.7.14 for OSX (dmg)**

1. Download the dmg file and install it

#. During the installation, an initial password will be shown on the screen (usually the combination of some complex characters)

#. Start MySQL service

|

**If you want to change the password for root**

- If you forget the initial password for root
    
    a\) Create a file abc (the filename is arbitrary) with the content: 
     
        **ALTER USER 'root'@'localhost' IDENTIFIED BY 'MyNewPass';**

        |
    
    b\) Start the MySQL server with the special --init-file option:               
    
        **mysqld_safe --init-file=/home/me/mysql-init &**

|

- If you remeber the initial password for root

    a\) Log in and enter the command to change the password: 
    
        **ALTER USER user IDENTIFIED BY 'MyNewPass';**
