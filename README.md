# HTTP Client integration tests

[![Latest Version](https://img.shields.io/github/release/php-http/client-integration-tests.svg?style=flat-square)](https://github.com/php-http/client-integration-tests/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)
[![Total Downloads](https://img.shields.io/packagist/dt/php-http/client-integration-tests.svg?style=flat-square)](https://packagist.org/packages/php-http/client-integration-tests)

**HTTP Client integration tests.**


## Install

Via Composer

```bash
composer require php-http/client-integration-tests
```


## Usage

This package should not be used on its own. It provides integration tests for HTTP Clients.


### Running tests for HTTP Adapters

Start the HTTP Test server:

```bash
vendor/bin/http_test_server
```

Install an adapter.

```bash
composer require php-http/curl-client laminas/laminas-diactoros
```

Run the tests.

```bash
./vendor/bin/phpunit --testsuite curl --printer "Http\Client\Tests\ResultPrinter"
```


## Contributing

Please see our [contributing guide](http://docs.php-http.org/en/latest/development/contributing.html).


## Security

If you discover any security related issues, please contact us at [security@php-http.org](mailto:security@php-http.org).


## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
