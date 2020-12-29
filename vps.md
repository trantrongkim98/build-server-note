# Config VPS server

## MYSQL

- sign in mysql

 ```sql
  mysql -u root -p

 ```

- create databse

```sql
CREATE DATABASE dbName
```

- show all databases

```sql
show databases;
show tables;
```

- import file

```sql
 mysql -u root -p dbName < file.sql 
```

## Command Start/Stop a thread in vps

### FIX ERROR

- could not find driver (SQL: select * from `meta` where `slug` = / limit 1)

```bash
yum install php-pdo
yum install php-pdo_mysql

service httpd restart
```

- start a service in vps

```bash
 nohup php -S 0.0.0.0:port
```

- find a process id of service

```bash
 netstat -tulpn
```

- stop service running

```bash
  kill PID
```

- login mysql

```bash
 mysql -u user -p
```

 then

```bash
 press password
```
