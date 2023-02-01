# Bacularis
Interface grafica do bacula

Instalar pacotes	(Debian 11)

apt install -y php7.3-bcmath php7.3-curl php7.3-xml  php7.3-ldap php7.3-mysqlnd php7.3-pdo php7.3-pgsql php7.3-intl


wget -qO- https://pkgs.bacularis.app/bacularis.pub | gpg --dearmor > /usr/share/keyrings/bacularis-archive-keyring.gpg


/etc/apt/sources.list.d/bacularis.list


Debian 11 Bullseye


deb [signed-by=/usr/share/keyrings/bacularis-archive-keyring.gpg] https://pkgs.bacularis.app/stable/debian bullseye main
deb-src [signed-by=/usr/share/keyrings/bacularis-archive-keyring.gpg] https://pkgs.bacularis.app/stable/debian bullseye main


Apache web server

apt install apache2

apt install bacularis bacularis-apache2

a2enmod rewrite

a2enmod proxy_fcgi

a2enconf php7.3-fpm

a2ensite bacularis

systemctl restart apache2

Access URL: http://seuhost:9097

Login: admin

Password: admin

Configurar API
