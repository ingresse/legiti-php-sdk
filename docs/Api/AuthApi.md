# Swagger\Client\AuthApi

All URIs are relative to *https://legiti-api.lgtcdn.net*

Method | HTTP request | Description
------------- | ------------- | -------------
[**auth**](AuthApi.md#auth) | **POST** /ticketing/v1/auth | Add a use auth operation and result

# **auth**
> \Swagger\Client\Model\CollectionSuccess auth($body)

Add a use auth operation and result

Account login/logout behavior is highly correlated with fraudulent activity. You can send information about successful or failed login attempts for an account (as well as logouts).

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: bearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\Auth**](../Model/Auth.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\CollectionSuccess**](../Model/CollectionSuccess.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

