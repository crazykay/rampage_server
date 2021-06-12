# rampage_server

#### Docker mysql container

```

docker run -itd --name winbest-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root mysql:latest

docker exec -it winbest-mysql bash -l

```

certbot certonly --manual --manual-auth-hook /etc/letsencrypt/acme-dns-auth.py --preferred-challenges dns --debug-challenges -d \*.your-domain -d your-domain

docker exec winbest-mysql /usr/bin/mysqldump -u root --password=root winbest > backup_2021-02-27.sql
