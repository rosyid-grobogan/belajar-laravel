# Artisan

Pembuatan Controller

```php
php artisan make:controller PostController
```

Pembuatan Model

```
php artisan make:model Post
```

Pembuatan Migration

```php
php artisan make:migration create_posts_table
```

Cara Singkat

```php
// see more
php artisan make:model -h
php artisan make:model Post -mc
```

| No  | Option | Option       | Description                                                                       |
| --- | ------ | ------------ | --------------------------------------------------------------------------------- |
|     | -a     | --all        | Generate a migration, seeder, factory, and resource controller for the model      |
|     | -c     | --controller | Create a new controller for the model                                             |
|     | -f     | --factory    | Create a new factory for the model                                                |
|     |        | --force      | Create the class even if the model already exists                                 |
|     | -m     | --migration  | Create a new migration file for the model                                         |
|     | -s     | --seed       | Create a new seeder file for the model                                            |
|     | -p     | --pivot      | Indicates if the generated controller should be a custom intermediate table model |
|     | -r     | --resource   | Indicates if the generated controller should be a resource controller             |
|     |        | --api        | Indicates if the generated controllr should be an API controller                  |
|     | -h     | --help       | Display this help message                                                         |
|     | -q     | --quiet      | Do not output any message                                                         |
|     | -v     | --version    | Display this application version                                                  |
