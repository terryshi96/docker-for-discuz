# docker-for-discuz
docker-compose file for discuz

##Usage
```
chmod -R 777 discuz/html
docker-compose up -d
and visit localhost:port to install
```

##configuration
```
discuz/config/php.ini is for php
discuz/html  is the source code and discuz configuration
```
```
in docker-compose.yml you can change
mysql configuration
port mapping
```

##make sure database host is mariadb
