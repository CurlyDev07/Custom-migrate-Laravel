# Custom-migrate-Laravel
Laravel Custom DB Migrate


Laravel Custom DB Migrate allows fine grain control of migrations inside your Laravel or Lumen application. You can choose which migration files - or groups of files inside the directory - get migrated to the database.

**********************_Installation_**********************
You can install the package via composer:
*** run
composer require sayeed/custom-migrate


***Laravel 5.5 and above
The package will automatically register itself, so you can start using it immediately.


***USAGE

After installing the package, you will now see a new php artisan migrate:custom command.

Migrate specific file
You can migrate a specific file inside your database/migrations folder using:

php artisan migrate:custom -f 2018_10_14_054732_create_tests_table

Alternatively, you can use the longform version:

php artisan migrate:custom --file 2018_10_14_054732_create_tests_table

Migrate specific directory
You can migrate a specific directory inside your database/migrations folder using:

php artisan migrate:custom -d migrations-subfolder

Alternatively, you can use the longform version:

php artisan migrate:custom --directory migrations-subfolder

Refreshing migrations
You can refresh migrations inside your project using:

php artisan migrate:custom -r

Alternatively, you can use the longform version:

php artisan migrate:custom --refresh
