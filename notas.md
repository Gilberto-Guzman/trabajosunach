# Comandos:

### Creación y configuración del proyecto.

    composer create-project laravel/laravel trabajosunach
    composer require laravel/breeze --dev
    php artisan breeze:install

    php artisan list
    php artisan route:list

    git clone https://github.com/MarcoGomesr/laravel-validation-en-espanol.git resources/lang

    php artisan make:component link
    php artisan make:migration add_rol_to_users_table
    php artisan migrate

    php artisan make:controller VacanteController -r
    php artisan make:model Vacante
    php artisan make:migration create_vacante_table --create=vacantes

    composer require livewire/livewire

    php artisan make:livewire CrearVacante
    php artisan make:seeder SalarioSeeder
    php artisan make:migration create_salarios_table
    php artisan migrate

    /*Los seeders se utilizan para manjear datos no dinamicos*/
    php artisan db:seed
    php artisan make:model Salario

    php artisan make:seeder CategoriasSeeder
    php artisan make:migration create_categorias_table

    php artisan migrate
    php artisan db:seed
    php artisan migrate:rollback
    php artisan migrate:rollback
    php artisan migrate
    php artisan db:seed
    php artisan make:model Categoria

    php artisan make:livewire MostrarAlerta

    php artisan migrate
    php artisan migrate:rollback
    php artisan migrate

    php artisan migrate:rollback
    php artisan migrate

    php artisan migrate:rollback
    php artisan migrate
    php artisan db:seed

    php artisan make:migration add_columns_to_vacantes_table

    php artisan migrate

    php artisan make:livewire MostrarVacantes
    php artisan vendor:publish --tag=laravel-pagination

### Enlaces.

1.  Página principal.

        http://trabajosunach.test/

2.  Herramienta de testeo de emails.

        http://mailhog:8025/

Nota: Para implementar mailhog en Laragon, requerirás configurarlo de esta manera:

    https://pen-y-fan.github.io/2023/01/04/how-to-set-up-laragon-on-a-new-windows-computer-part-5/#download-mailhog
