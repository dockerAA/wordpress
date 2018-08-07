# wordpress
nginx + php-fpm (wordpress) + mariadb

# random password
$ openssl rand -base64 32 > .secrets/mysql_root_password

# Strong SSL Security on nginx <br> 
Forward Secrecy & Diffie Hellman Ephemeral Parameters <br>
$ openssl dhparam -out dhparam.pem 4096 <br>
source: https://raymii.org/s/tutorials/Strong_SSL_Security_On_nginx.html <br>
ssl test: https://www.ssllabs.com/ssltest/ 

<br>
<br>
# Docker Container List (wordpress) <br>
1. nginx:1.13 ( 80:80 and 443:443) <br>
2. wordpress:4.9-php7.2-fpm (# 9000:9000 ) <br>
3. mariadb:10.2 (# 3306:3306 ) <br>
4. phpmyadmin/phpmyadmin:latest ( 9070:80 ) <br>
