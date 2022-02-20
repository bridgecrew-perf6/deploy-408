
# 1. Deploying Laravel using Envoy


## System Requirements
To be able to run Laravel Boilerplate you have to meet the following requirements:
- PHP >= 7.4
- PHP Extensions: BCMath, Ctype, Fileinfo, JSON, Mbstring, OpenSSL, PDO, Tokenizer, XML, cURL, Mcrypt, GD
- Node.js >= 8.x
- Composer >= 1.9.x

### 2.Local project setup



## 1.Install Composer using detailed installation instructions [here](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

```
wget https://getcomposer.org/composer.phar
chmod +x composer.phar
sudo mv composer.phar /usr/local/bin/composer
```
```
ssh -V
git clone https://github.com/Labs64/laravel-boilerplate.git dploy
cd dploy
sudo rm -rf .git
cp .env.example .env
composer install --prefer-dist
php artisan key:generate
npm install
npm run dev
php artisan migrate --seed
php artisan key:generate


```

### 3.Sever creation and firewall setup

```
sudo ufw enable
sudo ufw status
sudo ufw allow ssh
sudo ufw allow http
sudo ufw allow https
```

# 4.LEMP stack installation and setup


### 5.GIT repo setup and Nginx configuration
### 6.Install Laravel project on server
### 7.First project build on the live server
### 8.Laravel folder permissions and config file
### 9.Laravel production commands and migrations
### 10.Laravel Envoy installation and setup 
### 11.Linux Interactive shell potential pitfalls
### 12.Laravel Envoy deployment script
### 13.Creating Laravel Envoy stories

```




