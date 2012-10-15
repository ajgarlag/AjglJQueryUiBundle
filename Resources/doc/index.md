Getting Started With AjglJQueryUiBundle
=======================================

The AjglJQueryBundle adds **jQuery Ui** javascript library to **Symfony2**.

## Prerequisites

This version of the bundle has been tested with Symfony 2.1.


## Installation

Installation is a quick process:

1. Download AjglJQueryUiBundle using composer
2. Enable the Bundle

### Step 1: Download AjglJQueryUiBundle using composer

Add AjglJQueryUiBundle in your composer.json:

```js
{
    "require": {
        "ajgl/jqueryui-bundle": "*"
    }
}
```

Now tell composer to download the bundle by running the command:

``` bash
$ php composer.phar update ajgl/jqueryui-bundle
```

Composer will install the bundle to your project's `vendor/ajgl` directory.

### Step 2: Enable the bundle

Enable the bundle in the kernel:

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Ajgl\Bundle\JQueryUiBundle\AjglJQueryUiBundle(),
    );
}
```

### Next Steps

Now that you have completed the basic installation you should include the
required script tags in your templates