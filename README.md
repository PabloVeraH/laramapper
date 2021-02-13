# Laravel 6 Google Maps

Se usa como frontend este tema [WordPress gratis](https://wpgeodirectory.com/downloads/directory-starter/).
Hecho con La verion 6 de Laravel

## Características

- Administrador usa Google Places API
- Administrador usa [Spatie Opening Hours package](https://github.com/spatie/opening-hours) para manejar horas de atencion
- En el front-end usa Google Maps API para ver la posicion geografica


## Como se usa

- Clonar el repositorio (git clone)
- Copie el archivo __.env.example__ hacia __.env__ y edite las variables de coneccion y otras variables globales
- Ejecute __composer install__
- Ejecute __php artisan key:generate__
- RuEjecuten __php artisan migrate --seed__
- En el archivo __.env__ agregue su Google Maps API key: `GOOGLE_MAPS_API_KEY=AIzaSyBi2dVBkdQSUcV8_xxxxxxxxxxxx`
- Se puede loguear a la aplicacion en la URL `/login` URL poner las credenciales __admin@admin.com__ - __password__
- Se puede usar el archivo docker-compose para lanzar la aplicacion en local ejecutando ```docker-compose up -d``` si lo tiene instalado. Si no simplemente ejecute ```php artisan serve```