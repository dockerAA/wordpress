# README

## wordpress

nginx + php-fpm \(wordpress\) + mariadb + let's encrpyt \(ssl,tls\)

## random password

$ openssl rand -base64 32 &gt; .secrets/mysql\_root\_password

## Strong SSL Security on nginx  

Forward Secrecy & Diffie Hellman Ephemeral Parameters   
 $ openssl dhparam -out dhparam.pem 4096   
 source: [https://raymii.org/s/tutorials/Strong\_SSL\_Security\_On\_nginx.html](https://raymii.org/s/tutorials/Strong_SSL_Security_On_nginx.html)   
 ssl test: [https://www.ssllabs.com/ssltest/](https://www.ssllabs.com/ssltest/)

=======
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
5. certbot/certbot:latest (https://letsencrypt.org) <br>
release/v1.0.0
