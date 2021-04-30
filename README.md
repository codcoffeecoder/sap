Requirements 
Composer, PHP 7.3 above or 8.0, Mariadb / Mysql latest 

Steps
1. git clone this repo
3. cp .env.example .env
4. 
    - Might need to change the db credentials in .env file. 
    - Keep the CACHE_DRIVER to array, otherwise can use redis if there is.
    - APP_URL keeps as http://127.0.0.1:8000, assuming it will use an artisan server. If there is a virtual host provided, it will have to change this url similar to virtual host server name
5. composer install
6. php artisan key:gen
7. php artisan migrate
8. php artisan serve
9. Go to http://127.0.0.1:8000
10. Login as admin@email.com / admin123
