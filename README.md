FlameCore Webtools
==================

[![Latest Stable](http://img.shields.io/packagist/v/flamecore/webtools.svg)](https://packagist.org/packages/flamecore/webtools)
[![Build Status](https://img.shields.io/travis/FlameCore/Webtools.svg)](https://travis-ci.org/FlameCore/Webtools)
[![Code Climate](http://img.shields.io/codeclimate/github/FlameCore/Webtools.svg)](https://codeclimate.com/github/FlameCore/Webtools)
[![License](http://img.shields.io/packagist/l/flamecore/webtools.svg)](http://www.flamecore.org/projects/webtools)

This library provides common tools for working with web resources. The components are designed to be lightweight, fast and easy to use.

The Webtools package was developed for our linkparser framework [Flink](https://github.com/FlameCore/Flink) and the spam-protection
system [Gatekeeper](https://github.com/FlameCore/Gatekeeper).

Usage instructions and more information can be found [in our Wiki](https://github.com/FlameCore/Webtools/wiki).


Components
----------

* **UserAgent**

    Simple and fast User Agent string parser

* **WebpageAnalyzer**

    Get images, title and description of a webpage

* **HttpClient**

    Simple and intuitive HTTP Client

* **HtmlExplorer**

    Convenience wrapper for DOMDocument


Installation
------------

### Install via Composer

Create a file called `composer.json` in your project directory and put the following into it:

```
{
    "require": {
        "flamecore/webtools": "1.2.0"
    }
}
```

[Install Composer](https://getcomposer.org/doc/00-intro.md#installation-nix) if you don't already have it present on your system:

    $ curl -sS https://getcomposer.org/installer | php

Use Composer to [download the vendor libraries](https://getcomposer.org/doc/00-intro.md#using-composer) and generate the vendor/autoload.php file:

    $ php composer.phar install

Include the vendor autoloader and use the classes:

```php
namespace Acme\MyApplication;

use FlameCore\Webtools\HttpClient;
use FlameCore\Webtools\HtmlExplorer;

require_once 'vendor/autoload.php';
```


Requirements
------------

* You must have at least PHP version 5.4 installed on your system.


Contributors
------------

If you want to contribute, please see the [CONTRIBUTING](CONTRIBUTING.md) file first.

Thanks to the contributors:

* Christian Neff (secondtruth)
