# PHP Blog Project With Admin Dashboard

## Create Routing System 
- Create **.htaccess** file and paste some code
- `` 
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule ^(.*)$ index.php?url=$1 [L,QSA]
``
- Here URL is a variable which store on super global variable
- You check this `url` and redirect user needed page

## Database Design
We need a MySQL Database and 3 tables. 
1. users table `(id, username, email, password, date, role)`
2. categories table `(id, category_name, cateory_slug, disabled)`
3. posts table `(id,category_id, user_id, image, title, content, date, slug, date,)`