# My project

## SYSTEM REQUIREMENT

* DB: MySQL 5.6 
* Apache: 2.4 
* PHP: 7.0
* Laravel: 5.7 
* Composer: 1.4.1

## SETUP

* Clone
```bash
git clone https://github.com/hoangpham2395/chat.git
```

* Run
```bash
composer install
cp .env.example .env (CMD: copy .env.example .env)
php artisan key:generate
```

* Open file .env and config database
```bash
DB_DATABASE=homestead
DB_USERNAME=homestead
DB_PASSWORD=secret
```

* Delete cache
```bash
php artisan cache:clear
php artisan config:clear
php artisan view:clear
```

* Run migration
```bash
php artisan migrate
```

* Run seeder
```bash
php artisan db:seed
```

* Install redis
```bash
composer require predis/predis
```

* Install vuejs
```bash
npm install
```

## CONFIG URL

* C:\Windows\System32\drivers\etc\hosts
```bash 
127.0.0.1 dev.chat.vn
```

* C:\xampp\apache\conf\extra\httpd-vhosts.conf
```bash 
<VirtualHost *:80>
    DocumentRoot "{LOCAL_HTDOCS}\chat\public"
    ServerName dev.chat.vn
</VirtualHost>
<VirtualHost *:443>
    DocumentRoot "{LOCAL_HTDOCS}\chat\public"
    ServerName dev.xdmc.vn
    SSLEngine on
    SSLCertificateFile "C:\xampp\apache\conf\ssl.crt\server.crt"
    SSLCertificateKeyFile "C:\xampp\apache\conf\ssl.key\server.key"
</VirtualHost>
```

## RUN IN BROWSER

```bash 
dev.chat.vn
```