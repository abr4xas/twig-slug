## Twig Slug Generator

[![GitHub issues](https://img.shields.io/github/issues/abr4xas/twig-slug.svg?style=flat-square)](https://github.com/abr4xas/twig-slug/issues) [![GitHub forks](https://img.shields.io/github/forks/abr4xas/twig-slug.svg?style=flat-square)](https://github.com/abr4xas/twig-slug/network) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://raw.githubusercontent.com/abr4xas/twig-slug/master/LICENSE)


A [Twig](http://twig.sensiolabs.org/) extension for [abr4xas/twig-slug](https://github.com/abr4xas/twig-slug).

## how to install

```bash
$ composer require abr4xas/twig-slug
$ composer dumpautoload -o // optional
```


## usage

First register the extension with Twig:

```php
$twig = new Twig_Environment($loader);
$twig->addExtension(new \SeoUrl\SeoUrl());
```

Then use it in your templates:

```
{{ This is an awesome string | seourl }} // output: this-is-an-awesome-string
```

In `SomeController` like this:

```php
<?php

namespace SomeNameSpace;

use SeoUrl\SeoUrl;

class SomeController
{
    public function someFunction()
    {
        $str = 'This is an awesome string';

        $seoUrl = SeoUrl::generateSlug($str); // output: this-is-an-awesome-string

    }
}
```