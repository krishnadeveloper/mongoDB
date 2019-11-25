# mongoDB Backup on AWS - Ubuntu

### Process to check database on server
  
  1. Open Terminal
  2. Connect to server from `terminal` or windown `cmd`
  3. Connect to mongodb `mongo -u username -p password --authenticationDatabase your_database_name`
  4. Check your database after login on mongodb
  5. Run `exit` to logout from mongo

### Create a backup directory on server
  
  1. You must be connected with srever or follow the steps explained above
  2. Create backup directory 
     ```
     > cd /var/www/html
     > mkdir backups
     > cd ~
     OR
     > cd
     ```
  3. Run below command to create backup 
  
     ```
     1. Secure-DB backup command
     
     > mongodump -d you_DB_name -o ~/var/www/html/backups/first_backup -u username -p password --authenticationDatabase you_DB_name
     
     1. Non-Secure-DB backup command
     
     > mongodump -d you_DB_name -o ~/var/www/html/backups/first_backup
     
     ```
  4. Go Backup directory
      
      ```
      > cd var/www/html/backups/first_backup (Move to backup directory)
      > ls (you_DB_name directory will appear will all collections after run the command)
      > cd you_DB_name (Complete backup will be inside you_DB_name directory)
      ```

### Conclusion 
    You have taken the backup of you selected database
 
