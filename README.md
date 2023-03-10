# Template Laravel9 + Bootstrap + SASS

Istruzioni da eseguire al terminale per risolvere l'errore 500
composer install 
mv .env.example .env 
php artisan cache:clear 
composer dump-autoload 
php artisan key:generate


Oggi facciamo la nostra prima vera interazione con il database utilizzando l'ORM di Laravel.

1 - Create un nuovo progetto Laravel 9

2 - tramite phpMyAdmin create un nuovo database laravel_model_controller

3 - Importate nel vostro database la tabella movies in allegato

4 - inserite le vostre credenziali per il database nel file .env

5 - Create un model Movie
php artisan make:model Movie

6 - Create un controller che gestirà la rotta /
php artisan make:controller Guest/PageController

7 - All'interno della funzione index() del controller, recuperate tutti i film dal database e passateli alla view, che quindi li visualizzerà a schermo, tramite delle card.

BONUS:
Stilare il layout nei dettagli con Sass