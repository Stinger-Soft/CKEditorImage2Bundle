# CKEditor plugin Image2 Bundle for Symfony2
Symfony2 Bundle to integrate the CKEditor plugin Image2

## Current Version

Image2 v4.4.8

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-image2-bundle": "~4.4.8"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\CKEditorImage2Bundle\StingerCKEditorImage2Bundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-image2-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      image2:
        path: 'bundles/stingerckeditorimage2'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/image2
2. http://symfony.com
