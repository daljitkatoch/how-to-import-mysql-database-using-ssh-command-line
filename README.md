# Importing MySQL Databases via SSH

To manage databases without a control panel, you need to use the SSH command line to import. SQL backup files. These are the steps to import sql dump using putty or Ssh terminal

1. Connect to putty using ppk file
2. Log in to SSH as the root user
3. To log in to MySQL, Enter the following commands 
  
    a) **mysql -u username -p**
  
    b) Now You will asked for the enter password. Enter Password of DB's user and Press Enter
  
    c) **USE databasename;**
  
    d) Type **SOURCE /path/to/sql/dump.sql** and then press enter
  
    e) Monitor the running import log to check for errors
  
    f) To confirm the data was imported correctly, type **show tables;** and then press Enter
  
    g) Type **select * from tablename;** and then press Enter. Your imported MySQL database tables display.
  
That's All. You are done.






