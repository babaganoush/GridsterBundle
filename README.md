# Gridster Bundle for Symfony2

## Current Version

gridster.js - v0.5.6 - 2014-09-25

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "babaganoush/gridster-bundle": "dev-master"
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
        new Babaganoush\GridsterBundle\BabaganoushGridsterBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update babaganoush/gridster-bundle
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
<link rel="stylesheet" type="text/css" href="{{ asset('bundles/babaganoushgridster/css/jquery.gridster.css') }}" />
```

The Gridster scripts requires jQuery. The bundle installs bmatzner/jquery-bundle, which should be referenced before
loading any foundation script.

``` html
<script type="text/javascript" src="{{ asset('bundles/bmatznerjquery/js/jquery.min.js') }}"></script>
<script type="text/javascript" src="{{ asset('bundles/babaganoushgridster/js/jquery.gridster.js') }}"></script>
```


## Licenses

Refer to the source code of the included files for license information

## References

1. http://gridster.net/
2. http://symfony.com


