# Laravel Model Encryptable

Laravel Model Encryptable is a trait for Laravel Model that automatically encrypt attributes when save and decrypt attributes when retrieve

# Installation

Simply add the following line to your `composer.json` and run `composer update`

```
"arzeroid/laravel-model-encryptable": "^1.0",
```

Or use composer to add it with the following command

```
composer require "arzeroid/laravel-model-encryptable"
```

# Usage

Add the trait to your model and set your attributes to be encrypted in **encryptable** array

```php
<?php

namespace App\Models;

use Arzeroid\LaravelModelEncryptable\Encryptable;

class ActualPersonalCost extends BaseModel
{
    ...
    use Encryptable;
    
    /**
     * The attributes that should be encrypted.
     *
     * @var array
     */
    protected $encryptable = [
        'cost',
    ];

    ...
}
```
