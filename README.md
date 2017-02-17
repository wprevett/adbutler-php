# AdButler PHP bindings

[![Travis](https://img.shields.io/travis/adbutler/adbutler-php.svg?style=flat-square)](https://travis-ci.org/adbutler/adbutler-php)
[![Packagist Pre Release](https://img.shields.io/packagist/vpre/adbutler/adbutler-php.svg?style=flat-square)](https://packagist.org/packages/adbutler/adbutler-php)
[![Total Downloads](https://img.shields.io/packagist/dt/adbutler/adbutler-php.svg?style=flat-square)](https://packagist.org/packages/adbutler/adbutler-php)
[![License](https://img.shields.io/github/license/adbutler/adbutler-php.svg?style=flat-square)](https://github.com/adbutler/adbutler-php/blob/master/LICENSE)

You can sign up for an AdButler account at [https://adbutler.com](https://adbutler.com).

If you are looking for documentation, go here: [https://adbutler.com/docs/api?php](https://adbutler.com/docs/api?php)

## Beta
This project is currently in closed beta, but is considered fully functional.
You may request an API key here: [https://getfoureyes.com/s/a3leK/](https://getfoureyes.com/s/a3leK/)

## Requirements
  1. [AdButler account](https://adbutler.com/)
  2. PHP 5.3.3 or later

## Installation

### Composer

You can install the bindings via [Composer](http://getcomposer.org/).
Run the following command:

```bash
composer require adbutler/adbutler-php
```

To use the bindings, use Composer's [autoload](https://getcomposer.org/doc/00-intro.md#autoloading):

```php
require_once('vendor/autoload.php');
```

### Manual Installation

If you do not wish to use Composer, you can download the
[latest release](https://github.com/adbutler/adbutler-php/releases).
Then, to use the bindings, include the `init.php` file.

```php
require_once('/path/to/adbutler-php/init.php');
```

## Getting Started

Simple usage looks like:

```php
\AdButler\API::init(array('api_key' => '45e8fca2dc0f896fd7cb4cb0031ba249'));

$advertiser = \AdButler\Advertiser::create(array(
  "can_change_password" => true,
  "can_add_banners" => true,
  "email" => "demo.advertiser@adbutler.com",
  "name" => "Demo Advertiser",
  "password" => "some_password"
));

echo $advertiser;
```

## Documentation

Please see https://adbutler.com/docs/api for up-to-date documentation.

## License
© 2016–2017 SparkLIT. Released under the MIT license.
