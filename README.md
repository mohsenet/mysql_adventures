# mysql_adventures

### Export desired table from database
```bash
mysqldump -u root -p database_name table_name > table_name_backup.sql
```
### Import desired table from database
```bash
mysql -u root -p database_name < table_name_backup.sql
```

# Query limited

### Show top of the table
```bash
select * from table_name ORDER BY id DESC 5;
```
### Show tail of the table
```bash
select * from table_name ORDER BY id DESC LIMIT 5;
```

# Create database

```bash
CREATE DATABASE mydatabase CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

