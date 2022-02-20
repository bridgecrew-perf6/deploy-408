
# 1. Deploying Laravel using Envoy


## System Requirements
To be able to run Laravel Boilerplate you have to meet the following requirements:
- PHP >= 7.4
- PHP Extensions: BCMath, Ctype, Fileinfo, JSON, Mbstring, OpenSSL, PDO, Tokenizer, XML, cURL, Mcrypt, GD
- Node.js >= 8.x
- Composer >= 1.9.x



## 2.Local project setup
### 1.Install Composer & nvm  [here](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)
### Composer install

```
wget https://getcomposer.org/composer.phar
chmod +x composer.phar
sudo mv composer.phar /usr/local/bin/composer

or

php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '906a84df04cea2aa72f40b5f787e49f22d4c2f19492ac310e8cba5b96ac8b64115ac402c8cd292b8a03482574915d1a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer

```
### nvm install

```

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm

nvm -v
nvm install node 
node -v
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
==> 

php artisan migrate --seed
php artisan serve

```

### 3.Sever creation and firewall setup

```

sudo ufw app list
sudo ufw status
sudo ufw allow ssh
sudo ufw allow http
sudo ufw allow https
```

# 4.LEMP stack installation and setup

```
adduser mark
usermod -aG sudo mark
rsync --archive --chown=mark:mark ~/.ssh /home/mark

sudo apt install ngnix
sudo apt install mysql-server
sudo apt install php-fpm php-mysql php-dom php-mbstring php-cli php-zip wget unzip php7.4-xml -y


```

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




