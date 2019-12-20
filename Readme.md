1. create dhparam: openssl dhparam -out dhparam.pem 2048
2. install https://github.com/carlos-wong/certbot-dns-aliyun
3. certbot certonly -a certbot-dns-aliyun:dns-aliyun --certbot-dns-aliyun:dns-aliyun-credentials credentials.ini -d "testcertbot.lejuhub.com"
 
  3.1 credentials.ini is the config file for  https://github.com/carlos-wong/certbot-dns-aliyun
  
4. goto /etc/letsencrypt/live/domain
5. cp privkey.pem ~/sdc/test_nginx/ssl/star_forgott_com.key cp 
6. fullchain.pem ~/sdc/test_nginx/ssl/star_forgott_com.crt
7. start the docker-compose

