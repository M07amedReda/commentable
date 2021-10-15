# Laravel Commentable


## Installation

Require this package, with [Composer](https://getcomposer.org/), in the root directory of your project.

``` bash
$ composer require mohamedreda/commentable
```

To get started, you'll need to publish the vendor assets and migrate:

```
php artisan vendor:publish --provider="MohamedReda\Commentable\CommentableServiceProvider" && php artisan migrate
```

## Usage


### Setup a Model
``` php
<?php

namespace App;


use MohamedReda\Commentable\Traits\HasComments;
use Illuminate\Database\Eloquent\Model;

class Post extends Model
{
    use HasComments;
}
```