# Backbone.js Bundle for Symfony2

## Current Version

backbone.js v1.3.2

## Requirements

Backbone requires either Underscore.js or Lo-Dash and optionally jQuery or Zepto.

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/backbone-bundle": "~1.3"
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
        new Bmatzner\BackboneBundle\BmatznerBackboneBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/backbone-bundle
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

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<script type="text/javascript" src="{{ asset('bundles/bmatznerbackbone/js/backbone.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://documentcloud.github.com/backbone/
2. http://symfony.com
