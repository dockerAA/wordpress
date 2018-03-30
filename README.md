# wordpress
nginx + php-fpm (wordpress) + mariadb

# random password
$ openssl rand -base64 32 > .secrets/mysql_root_password

# Strong SSL Security on nginx <br> 
Forward Secrecy & Diffie Hellman Ephemeral Parameters <br>
$ openssl dhparam -out dhparam.pem 4096 <br>
source: https://raymii.org/s/tutorials/Strong_SSL_Security_On_nginx.html <br>
ssl test: https://www.ssllabs.com/ssltest/ 
