## Insatll mysqlclient and mariadb


### Befor install mysqlclient
```bash
sudo apt install build-essential python3-dev default-libmysqlclient-dev 
sudo apt install pkg-config
export MYSQLCLIENT_CFLAGS=`pkg-config mysqlclient --cflags`
export MYSQLCLIENT_LDFLAGS=`pkg-config mysqlclient --libs`
pip install mysqlclient
```

### Install mariadb on ubuntu
```bash
# https://www.digitalocean.com/community/tutorials/how-to-install-mariadb-on-ubuntu-20-04
sudo apt install mariadb-server
sudo mysql_secure_installation
mysql -uroot -p***** -e "create database YOUR_DATABASE_NAME character set utf8mb4 collate utf8mb4_unicode_ci;"
# get mariadb vertion
SELECT @@version;
# or
sudo mysqladmin version
```

