# Vue 3 in Laravel 10

Minimal Vue 3 application with router, i18n, pinia store.

## Install package

```sh
composer create-project laravel/laravel:^10.0 vue-app
cd vue-app
```

### Overwrite files
Backup first ***routes*** and ***resources*** directory!

```sh
php artisan vendor:publish --tag=vue-config --force
```

### Build and run app

```sh
npm install
npm run build
php artisan serve --host=localhost --port=8000
```

## Remove package
The package is no longer needed.

```sh
composer remove oleksandr/Proj-Laravel-Vue
```

## (DEV) Local repository import

Package directory: packages/oleksandr/Proj-Laravel-Vue

### Laravel composer.json

```json
{
    "repositories": [{
        "type": "path",
        "url": "packages/oleksandr/Proj-Laravel-Vue"
    }],
    "require": {
        "oleksandr/Proj-Laravel-Vue": "dev-main"
    },
}
```

### Vue3 npm packages

```sh
npm install vue@next
npm install vue-router@4
npm install vue-i18n@9
npm install --save-dev @vitejs/plugin-vue
npm install pinia
npm install @googlemaps/js-api-loader
```
