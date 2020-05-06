# Docker_Project

This project can launch a wordpress server with mysql database server on top of docker using docker compose.


Environment Details:--

1. Host os Red Hat Enterprise Linux : v8 (RHEL:V8).

2. docker-compose version 1.25.5

3. Docker version 19.03.8

4. Wordpress Docker image Wordpress:5.1.1-php.7.3-Apache

5. MySql Docker image mysql:5.7


If launched on LAN, it can be accessed by any any device across that particular lan.



Usage:--

   Clone the repo on local machine and run...

1. To launch for first time           "docker-compose up" .

2. To shutdown whole environment      "docker-compose stop" .

3. To relaunch environment            "docker-compose start"



Wordpress server is exposed to port 8080.



Seperate volumer are mounted to both the server for data security.

1. Volume "wordpressdrive" mounted to "/var/www/html" in Apache(httpd) server.

2. Volume "mysqldrive" mounter to "/var/lib/mysql" in mysql server.



Default parameters:--

MySql Server
1. ROOT_PASSWORD: root
2. USER: usr
3. PASSWORD: password
4. DATABASE: wordpressdatabas

