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


## nignx
```
upstream your_domain_name {
    server 127.0.0.1:port;
}
server
{

    listen       80;
    server_name your_domain_name;
    location / {
    proxy_set_header  X-Real-IP  $remote_addr;
    proxy_set_header  X-Forwarded-For $proxy_add_x_forwarded_for;
    proxy_set_header Host $http_host;
    proxy_redirect off;
    proxy_pass http://your_domain_name;
    }

}
```
