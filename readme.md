<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Laravel Excel Export Import

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

<ol>
    <li>download or clone project</li>
    <li>Go to the folder application using cd</li>
    <li>Run composer install on your cmd or terminal</li>
    <li>Copy .env.example file to .env on root folder.You can type copy .env.example .env if using command prompt Windows</li>
    <li>Open your .env file and change the database name (DB_DATABASE)</li>
    <li>Run php artisan key:generate</li>
    <li>Run php artisan migrate</li>
    <li>Run php artisan serve</li>
</ol>

####This Excample Laravel 5.8 Excel - Import Export

```
composer require "maatwebsite/excel:~2.1.0"
```

<p>In Config / app.php</p>

```php

 Maatwebsite\Excel\ExcelServiceProvider::class,

 Laravel\Tinker\TinkerServiceProvider::class,

'Excel' => Maatwebsite\Excel\Facades\Excel::class,

```

<p>Create DataBase Table</p>

```

php artisan make:migration create_cache_table --create=cache

php artisan make:migration create_books_table --create=books

```

<p>Create Controller</p>

```

php artisan make:controller BookController

```
<p> Create Model </p>

```

php artisan make:model Author

php artisan make:model Book

```
