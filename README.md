# mysql_adventures

### Export desired table from database
```bash
mysqldump -u root -p database_name table_name > table_name_backup.sql
```
### Import desired table from database
```bash
mysql -u root -p database_name > table_name_backup.sql
```

