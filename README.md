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
