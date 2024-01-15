## php-simple-html-dom-parser
==========================

Version 1.9.1

Adaptation for Composer and PSR-0 of:

A HTML DOM parser written in PHP5+ let you manipulate HTML in a very easy way!
Require PHP 5+.
Supports invalid HTML.
Find tags on an HTML page with selectors just like jQuery.
Extract contents from HTML in a single line.

http://simplehtmldom.sourceforge.net/


Install
-------
add to `composer.json`
```json
"require": {
    "camilord/php-simple-html-dom-parser": "1.9.1"
    }
```

or cast a command:
```bash
php composer.phar require camilord/php-simple-html-dom-parser
```

Usage
-----

```php
use camilord\HtmlDomParser;

...
$dom = HtmlDomParser::str_get_html($str);
or 
$dom = HtmlDomParser::file_get_html($file_name);

$elems = $dom->find('small.count');
...

```