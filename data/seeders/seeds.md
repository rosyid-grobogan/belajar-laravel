## Seeds



## Membuat Seeder

```
php artisan make UsersTableSeeder
```

Akan dibuatkan file `UsersTableSeeder.php` dan ditempatkan di direktori `database/seeds`.

## Membuat Data Dummy

```php
<?php

use Illuminate\Database\Seeder;
// Add Model
use App\Models\User;

class UsersTableSeeder extends Seeder
{
    /**
     * Run the database seeds.
     *
     * @return void
     */
    public function run()
    {
        // Kode Dummy
        $adminUser = [
            'name' => 'Admin',
            'email' => 'admin@abc.com',
            'password' => bcrypt('admin'),
        ];

        if ( !User::where('email', $adminUser['email'])->exists() ) {
            User::create($adminUser);
        }
    }
}

```

- Add Model
- Kode Dummy

## Daftarkan Seeder

di `database/seeds/DatabaseSeeder.php`

```php
    public function run()
    {
        // daftarkan
         $this->call(UsersTableSeeder::class);
    }
```



## Cara Menggunakan Seeder

```
php artisan db:seed
```

Perintah ini akan mengenerate data dummy yang sudah kita buat.



## Contoh Kode Seeder

```php
'name' => $faker->randomElement(['Scarves', 'Clothing', 'Apparel']),
'parent_id' => $faker->numberBetween(1, 3),

```