# This package is compatible with Laravel 5.3

This package relies on <a href="http://php.net/manual/en/book.image.php">php-gd</a> extension. So, make sure it is installed on your machine.

# Installation
Clone the repository-

git clone https://github.com/jahid56/recaptcha.git

Then cd into the folder with this command-

cd recaptcha
Then do a composer install

composer install
Then create a environment file using this command-

cp .env.example .env
Then edit .env file with appropriate credential for your database server. Just edit these two parameter(DB_USERNAME, DB_PASSWORD).

Then create a database named todos and then do a database migration using this command-

php artisan migrate
Then change permission of storage folder using thins command-

(sudo) chmod 777 -R storage
At last generate application key, which will be used for password hashing, session and cookie encryption etc.

php artisan key:generate

Then, register keys for your site at https://www.google.com/recaptcha/admin

Then Write your Secret and Site key in .ev file

NOCAPTCHA_SECRET=[]
NOCAPTCHA_SITEKEY=[]

You are now Set to go.