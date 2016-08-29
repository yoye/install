# install
Dev environment
```shell
# PHP5.6
sudo add-apt-repository ppa:ondrej/php 
sudo apt-get update
sudo apt-get install php5.6 php5.6-fpm php-redis php5.6-mbstring php5.6-mysql php5.6-intl php5.6-curl php5.6-xml php5.6-apcu php5.6-gd php-xdebug php-gettext

# PHP7
sudo apt-get install php php-fpm php-mbstring php-mysql php-intl php-curl php7.0-xml php7.0-apcu php-gd

# NodeJS
sudo apt-get install nodejs npm

# Elasticsearch
sudo add-apt-repository -y ppa:webupd8team/java
sudo apt-get update
sudo apt-get -y install oracle-java8-installer
wget -qO - https://packages.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
echo "deb http://packages.elastic.co/elasticsearch/1.7/debian stable main" | sudo tee -a /etc/apt/sources.list.d/elasticsearch-1.7.list
sudo apt-get update
sudo apt-get -y install elasticsearch
sudo systemctl start elasticsearch
sudo systemctl enabled elasticsearch

# Nginx
sudo apt-get install nginx
sudo systemctl start nginx

# Mysql
sudo apt-get install mysql-server phpmyadmin
```
