# Manifest

Component for reading [phar.io](https://phar.io/) manifest information from a [PHP Archive (PHAR)](http://php.net/phar).

## Installation

You can add this library as a local, per-project dependency to your project using [Composer](https://getcomposer.org/):

    composer require phar-io/manifest

If you only need this library during development, for instance to run your project's test suite, then you should add it as a development-time dependency:

    composer require --dev phar-io/manifest


## Usage

```php
require __DIR__ . '/src/autoload.php';

$manifest = \PharIo\Manifest\ManifestLoader::fromFile(__DIR__ . '/tests/_fixture/phpunit-5.6.5.xml');

var_dump($manifest);
```
