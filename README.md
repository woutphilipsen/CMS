**Add following line to your php.ini file**

extension=php_xsl.dll

**Open terminal and cd into CMS**
**run:**

composer install

**open .env file & adjust settings for local database url:**

DATABASE_URL=mysql://root:@127.0.0.1:3306/the_spacebar

**startup local sql server**
**go back to terminal & run:**

  php bin/console doctrine:database:create

  php bin/console doctrine:migrations:migrate

  php bin/console doctrine:fixtures:load

**start up server at localhost:8000, run:**

symfony serve

**to unlock content management (admin user):**

username: admin1@thespacebar.com

pwd: engage

**some pages:**
  
  https://localhost:8000/account
  
  https://localhost:8000/admin/article
  
  https://localhost:8000/admin/article/new
  
  https://localhost:8000/admin/article/1/edit
  
  https://localhost:8000/admin/comment
  
  https://localhost:8000/register
  
  https://localhost:8000/login
  
  https://localhost:8000/logout
  
  
  
