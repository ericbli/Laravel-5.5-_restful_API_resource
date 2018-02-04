# Laravel-5.5-_restful_API_resource

composer create-project --prefer-dist laravel/laravel larticles
composer create-project --prefer-dist laravel/laravel phonebook

create database larticles;
php artisan make:migration create_articles_table --create=articles

  $table->string('title');
            $table->text('body');
------------------------------------------------------------------------------
			
			php artisan make:seeder ArticlesTableSeeder
			php artisan make:factory ArticleFactory
			php artisan make:model Article
			
			php artisan migrate
			php artisan db:seed
			
			php artisan make:controller ArticleController --resource
			php artisan make:resource Article

                        

			
			http://larticles/api/articles
			http://larticles/api/article/3
postaman   delete	http://larticles/api/article/4

head:  body:
Content-Type  application/json



			post    http://larticles/api/article
			 {"title": "AAAAAA",
        "body": "BBBBBB"}
			
			put    http://larticles/api/article
			
			 { "id":5,
      "title": "AAAAAA",
        "body": "BBBBBB"}

			
			---------------------------------------------------------------
			clone projects
			-----------------
			put it to www
			cd projects
			composer update --no-scripts
			copy .env.example .env
			config database setting
			php artisan key:generate
			php mysqladmin create database: laravelblog
			php artisan migrate
			
			
			
			产生假数据SEED:
			-------------
			 factory(App\User::class, 50)->create();
			 php artisan db:seed

		     php artisan make:model Test
			 
			---------------------------------------------------------------- 
			 Phonebook
			 
			npm install vue-router
			npm install bulma --save
			npm install
			in resource/assets/sass/app.scss add:
			----------------------------------
			 //Bulma
@import "~bulma/bulma";
			 --------------------------------
			 npm run watch
             in resource/assets/components/bootstrap.js delete:
			 ----------------------------------
			  require('bootstrap-sass');
             ----------------------------------
			 
			 http://localhost:8000/
			 create new file phone book.blade.php
			 html:5  CE
			 div#app  CE
			 link     CE
			 
			 php artisan make:model phonebook -m -r
			 php artisan migrate
			 
			 
			 
			 
			
