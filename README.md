Requirements 
Composer, PHP 7.3 above or 8.0, Mariadb / Mysql latest 

Steps
1. git clone https://github.com/codcoffeecoder/sap.git
2. cp .env.example .env
3a. Might need to change the db credentials in .env file. 
3b. Keep the CACHE_DRIVER to array, otherwise can use redis if there is.
3c. APP_URL keeps as http://127.0.0.1:8000, assuming it will use an artisan server. If there is a virtual host provided, it will have to change this url similar to virtual host server name
4. composer install
5. php artisan key:gen
6. php artisan migrate
7. php artisan serve
8. Go to http://127.0.0.1:8000
9. Login as admin@email.com / admin123
