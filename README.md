## Timezones -Laravel package example

###Setup

composer.json
```
"autoload": {
        "classmap": [
            "database"
        ],
        "psr-4": {
            "App\\": "app/",
            
            ...
            "NancyCoop\\Timezones\\": "packages/nancycoop/timezones/src"
            ...
        }
    },
    
```
```
composer dump-autoload
````

config/app.php
```
'providers' => [

        ...
        Laraveldaily\Timezones\TimezonesServiceProvider::class,
        ...
  ]
```

### Publish views

```
php artisan vendor:publish
```

Packagist version incoming

View on [laraveldaily.com]
[laraveldaily.com]: <http://laraveldaily.com/how-to-create-a-laravel-5-package-in-10-easy-steps/>
