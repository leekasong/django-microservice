# django with mysql

## containers
- mysql/mysql-server:8.0

## information

### mysql 8.0
mysql 8.0 uses caching_sha2_password as default authentication.
so if we avoid setting sh2 auth, we need to prepare serveral setting before run the container.

- set --default-authentication-plugin=mysql_native_password in docker compose yml
- install initsql to the mysql container to clear the auth settings.

refer to 
https://blusky10.tistory.com/362 
https://kogle.tistory.com/87

### vscode plugin
i used mysql plugin, https://marketplace.visualstudio.com/items?itemName=cweijan.vscode-mysql-client2




 