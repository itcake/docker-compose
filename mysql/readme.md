
#### start mysql server
> docker-compose up -d

#### enable remote connect
> all ip
``` mysql
update user set host = '%' where user = 'root';
```

> part ip
``` mysql
update user set host = '127.0.*.*' where user = 'root';
```

####  update password
> ALTER USER 'root' IDENTIFIED WITH mysql_native_password BY 'Mysql123!@#';
> flush privileges;

