# CRUD Pasos Laravel Livewire
CRUD con Livewire
## Pasos para Crear Módulos en Laravel + Livewire

### Comenzando 🚀

## Instalación Laravel + Jetstream + Livewire
A) - Creación del proyecto
```
laravel new example-app
```

B) - Descargar los paquetes de Jetstream
```
composer require laravel/jetstream
```

C) - Instalación Jetstream + Livewire
```
php artisan jetstream:install livewire
```

D)
```
npm install
npm run build
php artisan migrate
```

## Paso No. 1

_Crear el modelo + migration + controller tipo resource_

```
php artisan make:model nameModel -mcr
```

## Paso No. 2

_Configurar la migración, todas las configuraciones de la base de datos._

## Paso No. 3

_Ejecuta la migración_

```
php artisan migrate
```

## Paso No. 4

_Exponer los campos en el Modelo_

```
Ejemplo: protected $fillable = ['id', 'name'];
```

## Paso No. 5

_Crear la vista_

```
nameModule/index.blade.php
```

## Paso No. 6

_Crear el metodo index en el controller_

```
public function index()
{
    return view('nameModule.index');
}
```

## Paso No. 7

_Crear la ruta que apuente al controlador_

```
Route::get('/nameModule', [nameController::class, 'index']);
```

## Paso No. 8

_Crear el Livewire Component_

```
php artisan make:livewire nameModule/nameComponent
```

## Paso No. 9

_Configurar los metodos/funciones en nameComponent_

## Paso No. 10

_Configurar y crear las vistas de nameComponent_

## Lanza el Servidor 🚀

```
php artisan serve
```

## Autores ✒️

-   **Samir Vergara V** - _Desarrollo_ - [web-v2](https://github.com/web-v2)

### Desarrollado por

```
Samir Vergara V
```

## Laravel Sponsors

## License

    The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
