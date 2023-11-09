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

    php artisan make:livewire EditarVacante
    php artisan storage:link

    php artisan make:policy VacantePolicy --model=Vacante
    npm install sweetalert2
    npm install sass

    php artisan make:livewire MostrarVacante

    php artisan make:livewire PostularVacante

    php artisan make:migration create_candidatos_table
    php artisan make:controller CandidatoController --model=Candidato

    php artisan migrate

    php artisan make:notification NuevoCandidato
    php artisan notifications:table
    php artisan migrate

    php artisan make:controller NotificacionController --invokable

    php artisan make:middleware RolUsuario

    php artisan make:controller HomeController --invokable
    php artisan make:livewire HomeVacantes

    php artisan make:livewire FiltrarVacantes

    php artisan migrate:refresh
### Enlaces.

1.  Página principal.

        http://trabajosunach.test/

2.  Herramienta de testeo de emails.

        http://mailhog:8025/
        http://localhost:8025/

Nota: Para implementar mailhog en Laragon, requerirás configurarlo de esta manera:

    https://pen-y-fan.github.io/2023/01/04/how-to-set-up-laragon-on-a-new-windows-computer-part-5/#download-mailhog

### Error Storage link

En resumen hay que entrar a public y eliminar stoagre, luego ejecutar de nuevo php artisan storage:link

    https://stackoverflow.com/questions/49489549/laravel-app-storage-images-failed-to-load-and-redirect-to-404



### Extra

Les explico como descargar sweetAlert2 por medio del npm y su configuración, bueno al menos la forma que me funcionó.

1. Ejecutar el comando: npm install sweetalert2

2. Importar el scss y js en tu archvi app.js:

import Swal from 'sweetalert2/dist/sweetalert2.js'

import 'sweetalert2/src/sweetalert2.scss'

3. En la documentación de sweetAlert no viene, pero hay que poner el siguiente código en el app.js

window.Swal =Swal;
Swal.start(); 4. Si les marca error en los estilos sass de sweetAlert (al menos a mí me sucedió), tendrán que instalar sass

npm install sass --dev

Y eso sería todo, al menos esos fueron los pasos que seguí para que me funcionará



### Digital Ocean

    php artisan key:generate --show
    base64:jTf5GK4X1VmgUuZxOodYJU0xugyZ611J6w9GEdjnseY=

    php artisan migrate
    php artisan db:seed
