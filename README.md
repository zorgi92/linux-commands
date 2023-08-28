# linux-commands

------------/УСТАНОВКА Apache/ <br>                                                                                                                                                

sudo apt install apache2 <br>

sudo systemctl status apache2  - статус <br>
sudo systemctl stop apache2    - стоп <br>
sudo systemctl start apache2   - старт <br>
sudo systemctl restart apache2 - перезагрузка <br>
sudo systemctl disable apache2 - отключить автостарт Apache <br>
sudo systemctl enable apache2  - включить автостарт Apache <br>

/sudo ufw allow 'Apache' <br>
/sudo ufw status <br>

Configuration File (php.ini) Path	        /etc/php/7.4/apache2 <br>
Loaded Configuration File	                /etc/php/7.4/apache2/php.ini <br>
Scan this dir for additional .ini files  	/etc/php/7.4/apache2/conf.d <br>

Apache: этот профиль открывает порт 80 (обычный, не шифрованный веб-трафик). <br>
Apache Full: этот профиль открывает порты 80 (обычный, не шифрованный веб-трафик) и 443 (трафик шифруется с помощью TLS/SSL). <br>
Apache Secure: этот профиль открывает только порт 443 (трафик шифруется с помощью TLS/SSL). <br>
https://www.digitalocean.com/community/tutorials/apache-ubuntu-18-04-ru <br>

------------/------------/------------/------------/------------/------------/------------/------------/------------/ <br>

------------/УСТАНОВКА PHP 8.1/ <br>

sudo apt install -y lsb-release ca-certificates apt-transport-https software-properties-common gnupg2 <br>

echo "deb https://packages.sury.org/php/ $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/sury-php.list <br>

wget -qO - https://packages.sury.org/php/apt.gpg | sudo apt-key add - <br>

sudo apt update <br>

sudo apt -y install php8.1 <br>
sudo apt -y install php8.2 <br>

sudo apt -y install libapache2-mod-php8.1 <br>
sudo apt -y install libapache2-mod-php8.2 <br>

https://losst.pro/ustanovka-php-v-debian#%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0_PHP_80_%D0%B8_81 <br>

sudo a2dismod php8.1 - выключить эту версию PHP <br>
sudo a2enmod php8.2  - включить эту версию PHP <br>
sudo service apache2 restart - перезагрузить apache2 <br>
update-alternatives --config php <br>


sudo apt install php8.0 <br>
sudo apt install php8.0 libapache2-mod-php8.0 <br>
sudo apt install php8.0-curl <br>
sudo apt-get install php8.0-mbstring <br>
sudo service apache2 restart <br>

sudo apt install php8.0-fpm php8.0-gd php8.0-curl php8.0-mysql php8.0-dev php8.0-cli php8.0-common php8.0-mbstring php8.0-intl php8.0-zip php8.0-bcmath <br>

sudo apt-get install php8.0-xml <br>
php -i | grep -i curl <br>

Это может спасти вас: <br>
sudo add-apt-repository ppa:ondrej/php <br>
sudo apt update <br>
sudo apt install software-properties-common  <br>


------------/------------/------------/------------/------------/------------/------------/------------/------------/ <br>
