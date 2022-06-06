# slimphpApp

installiton instructions:

1. clone the project
``` 
git clone https://github.com/akram-tello/slimphpApp.git
```
3. run 
```
composer install
````
4. add .htaccess file on main root folder
5. add in the .htaccess file
```
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^ index.php [QSA,L]
````
5. add another .htaccess file on public folder
6. add in the .htaccess file
```
RewriteEngine on
RewriteRule ^$ index.php [L]
RewriteRule (.*) index.php?slim=$1 [L] 
````
7. run 
````
php -S localhost:8080

