Delivery
===

A share work-zone in symfony/angularjs.

Requires
===
- PHP 5.3.9
- Mysql 5.0


Installation
===
- php -r "readfile('https://getcomposer.org/installer');" | php
- php composer.phar install --optimize-autoloader
- php app/console doctrine:database:drop --force
- php app/console doctrine:database:create
- php app/console doctrine:schema:update --force
- php app/console assets:install
- php app/console doctrine:fixtures:load -n
- php app/console cache:clear --env=prod