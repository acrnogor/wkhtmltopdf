wkhtmltopdf
================

This repository contains the static compiled binaries from the [wkhtmltopdf project](http://wkhtmltopdf.org/).
More about the functionality of wkhtmltopdf and wkthmltoimage can be found there.

Binaries for __Microsoft Windows__, also installable with composer, can be found here: [github.com/wemersonjanuario/wkhtmltopdf-windows](https://github.com/wemersonjanuario/wkhtmltopdf-windows)

Binaries for __CentOS 7__, also installable with composer, can be found here: [github.com/rvanlaak/wkhtmltopdf-amd64-centos7](https://github.com/rvanlaak/wkhtmltopdf-amd64-centos7)

## Installation

_Hint_:
The version of the binary is equal to the git tag - to install the latest version, use '0.12.5'.

### Packagist

This package can be found on [Packagist](http://packagist.org) and installed with [Composer](https://getcomposer.org/).

And for _amd64_ with:

    php composer.phar require acrnogor/wkhtmltopdf "0.1"

The binary will then be located at:

    vendor/acrnogor/wkhtmltopdf/bin/wkhtmltopdf

Also a symlink will be created in your configured bin/ folder, for example:

    vendor/bin/wkhtmltopdf

### Usage

You can use the path constant to easily locate the binary in the PHP codebase: 

``` php
$path = Acrnogor\Wkhtmltopdf::PATH;
```

For realpath use following script

``` php
$realpath = realpath(Acrnogor\Wkhtmltopdf::PATH);
```
