# linux-commands

------------/УСТАНОВКА Apache/

sudo apt install apache2

sudo systemctl status apache2  - статус
sudo systemctl stop apache2    - стоп
sudo systemctl start apache2   - старт
sudo systemctl restart apache2 - перезагрузка
sudo systemctl disable apache2 - отключить автостарт Apache
sudo systemctl enable apache2  - включить автостарт Apache

/sudo ufw allow 'Apache'
/sudo ufw status

Configuration File (php.ini) Path	        /etc/php/7.4/apache2
Loaded Configuration File	                /etc/php/7.4/apache2/php.ini
Scan this dir for additional .ini files  	/etc/php/7.4/apache2/conf.d

Apache: этот профиль открывает порт 80 (обычный, не шифрованный веб-трафик).
Apache Full: этот профиль открывает порты 80 (обычный, не шифрованный веб-трафик) и 443 (трафик шифруется с помощью TLS/SSL).
Apache Secure: этот профиль открывает только порт 443 (трафик шифруется с помощью TLS/SSL).
https://www.digitalocean.com/community/tutorials/apache-ubuntu-18-04-ru
