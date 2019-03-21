# Install Laravel Collective form support
##### Current version 5.8.0

#### Edit composer.json file to require laravelcollective/html

```console
"require": {
    "laravelcollective/html": "*"
}
```

####  Update Composer from the Terminal

```console
composer update
```

#### Add provider and two aliases in the config/app.php

```console
  'providers' => [
    // ...
    Collective\Html\HtmlServiceProvider::class,
    // ...
  ],
  
  ...
  
  'aliases' => [
    // ...
      'Form' => Collective\Html\FormFacade::class,
      'Html' => Collective\Html\HtmlFacade::class,
    // ...
  ],
```
