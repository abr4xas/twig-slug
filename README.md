## Twig Slug Generator

[![GitHub issues](https://img.shields.io/github/issues/abr4xas/twig-slug.svg?style=flat-square)](https://github.com/abr4xas/twig-slug/issues) [![GitHub forks](https://img.shields.io/github/forks/abr4xas/twig-slug.svg?style=flat-square)](https://github.com/abr4xas/twig-slug/network) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://raw.githubusercontent.com/abr4xas/twig-slug/master/LICENSE)


## how to install

```bash
$ composer require abr4xas/twig-slug
$ composer dumpautoload -o // optional
```


## how to use 

```php
$view->addExtension(new Abr4xas\SeoUrl\SeoUrl());
```

```
{{ This is an awesome string | seourl }} // output: this-is-an-awesome-string
```
