# docker-for-discuz
docker-compose file for discuz

##Usage
```
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

##use nginx as proxy
```
upstream your_domain_name {
    server discuz_server_ip:port weight=10;
}
      server
      {
              listen       80;
              server_name your_domain_name;
      }
```
