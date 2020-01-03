bonjour
j'en suis au niveau d'installation make install
Lorsque je lance la commande make check , voici le résultat:

root@omnispqce:/var/www/html/conges# make check
App/Tools/check
PHP Warning: PHP Startup: Unable to load dynamic library 'pdo_mysql1 (tried: /usr/lib/php/20170718/pdo_mysql (/usr/lib/php/20170718/pdo_mysql 
: cannot open shared object file: No such file or directory), /usr/lib/php/20170718/pdo_mysql.so (/usr/lib/php/20170718/pdo_mysql.so: undefined symbol: mysqlnd_allocator)) in Unknown on line 0
     /env php
1/11/01tg: require_once(/var/www/html/conges/vendor/autoload.php): failed to open stream: No such file or directory in /var/www/html/conges 
/App/Tools/libraries on line 23
PHP Fatal error: require_once(): Failed opening required '/var/www/html/conges/vendor/autoload.php' (include_path=1.:/usr/share/php') in /var 
/www/html/conges/App/Tools/libraries on line 23
Makefile:15: recipe for target 'check' failed
make: *** [check' Error 255

le fichier pdo_mysql.so est bien présent dans l'emplacement /usr/lib/php/20170718/

Merci d'avance pour votre aide
