# README

## wordpress

nginx + php-fpm \(wordpress\) + mariadb

## random password

$ openssl rand -base64 32 &gt; .secrets/mysql\_root\_password

## Strong SSL Security on nginx  

Forward Secrecy & Diffie Hellman Ephemeral Parameters   
 $ openssl dhparam -out dhparam.pem 4096   
 source: [https://raymii.org/s/tutorials/Strong\_SSL\_Security\_On\_nginx.html](https://raymii.org/s/tutorials/Strong_SSL_Security_On_nginx.html)   
 ssl test: [https://www.ssllabs.com/ssltest/](https://www.ssllabs.com/ssltest/)

