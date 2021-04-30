Requirements 
Composer, PHP 7.3 above or 8.0, Mariadb / Mysql latest 

Steps
1. git clone this repo
1. cp .env.example .env
1. 
    - Might need to change the db credentials in .env file. 
    - Keep the CACHE_DRIVER to array, otherwise can use redis if there is.
    - APP_URL keeps as http://127.0.0.1:8000, assuming it will use an artisan server. If there is a virtual host provided, it will have to change this url similar to virtual host server name
1. composer install
1. php artisan key:gen
1. php artisan migrate
1. php artisan serve
1. Go to http://127.0.0.1:8000
1. Login as admin@email.com / admin123
