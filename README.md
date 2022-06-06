# slimphpApp

installiton instructions:

```
1. clone the project
2. run composer install
3. add .htaccess file on main root folder
4. add `RewriteEngine on
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^ index.php [QSA,L]` in the .htaccess file
5. add another .htaccess file on public folder
6. add `RewriteEngine on
RewriteRule ^$ index.php [L]
RewriteRule (.*) index.php?slim=$1 [L]` in the .htaccess file
7. run `php -S localhost:8080`

```
