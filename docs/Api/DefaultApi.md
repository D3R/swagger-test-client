# Swagger\Client\DefaultApi

All URIs are relative to *http://virtserver.swaggerhub.com/D3R/ServerNames/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createName**](DefaultApi.md#createName) | **GET** /get | Creates a new server name


# **createName**
> \Swagger\Client\Model\ServerName[] createName($count, $length)

Creates a new server name

Return a generated server name with various features depending on the options set

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$count = 1; // int | Pass an optional count to get more than one name generated
$length = 56; // int | Maximum length of the server name(s)

try {
    $result = $api_instance->createName($count, $length);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createName: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **count** | **int**| Pass an optional count to get more than one name generated | [optional] [default to 1]
 **length** | **int**| Maximum length of the server name(s) | [optional]

### Return type

[**\Swagger\Client\Model\ServerName[]**](../Model/ServerName.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

