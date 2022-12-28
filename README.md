# vesta-php-fpm-81
VestaCP PHP templates for PHP 8.1

Usage:

```
apt-get install php8.1-apcu php8.1-mbstring php8.1-bcmath php8.1-cli php8.1-curl php8.1-fpm php8.1-gd php8.1-intl php8.1-mysql php8.1-soap php8.1-xml php8.1-zip php8.1-memcache php8.1-memcached php8.1-zip
update-rc.d php8.1-fpm defaults
a2enconf php8.1-fpm
systemctl restart apache2
cp -r /etc/php/8.1/ /root/vst_install_backups/php8.1/
rm -f /etc/php/8.1/fpm/pool.d/*
wget https://github.com/t0rik/vesta-php-fpm-81/raw/master/PHP-FPM-81.stpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-81.stpl
wget https://github.com/t0rik/vesta-php-fpm-81/blob/master/PHP-FPM-81.tpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-81.tpl
wget https://raw.githubusercontent.com/t0rik/vesta-php-fpm-81/master/PHP-FPM-81.sh -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-81.sh
chmod a+x /usr/local/vesta/data/templates/web/apache2/PHP-FPM-81.sh
```
