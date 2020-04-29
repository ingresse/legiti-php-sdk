# SwaggerClient-php
Legiti protects your company from losses due to fraud and chargebacks, maximizing revenue from valid purchases and minimizing unnecessary customer friction. We accomplish this by making predictions based on past and present customer behavior to evaluate the likelihood that an order is fraudulent.

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0
- Build package: io.swagger.codegen.v3.generators.php.PhpClientCodegen

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/):

```
composer require ingresse/legiti-php-sdk
```

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new Swagger\Client\Api\AuthApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\Auth(); // \Swagger\Client\Model\Auth |

try {
    $result = $apiInstance->auth($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AuthApi->auth: ', $e->getMessage(), PHP_EOL;
}
?>
```

## Documentation for API Endpoints

All URIs are relative to *https://legiti-api.lgtcdn.net*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthApi* | [**auth**](docs/Api/AuthApi.md#auth) | **POST** /ticketing/v1/auth | Add a use auth operation and result

## Documentation For Models

 - [AccessError](docs/Model/AccessError.md)
 - [Auth](docs/Model/Auth.md)
 - [AuthorizationError](docs/Model/AuthorizationError.md)
 - [CollectionSuccess](docs/Model/CollectionSuccess.md)
 - [RequestError](docs/Model/RequestError.md)

## Documentation For Authorization


## bearerAuth

- **Type**: HTTP bearer authentication


## Author



