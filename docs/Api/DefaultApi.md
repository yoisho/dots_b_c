# Swagger\Client\DefaultApi

All URIs are relative to *https://bcd-web.net/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addObjectValueUsingPOST**](DefaultApi.md#addObjectValueUsingPOST) | **POST** /api/v1/user/objects/{objectId} | オブジェクトの登録
[**createAssetsUsingPOST**](DefaultApi.md#createAssetsUsingPOST) | **POST** /api/v1/user/assets | アセット作成
[**createNewAccountUsingPOST**](DefaultApi.md#createNewAccountUsingPOST) | **POST** /api/v1/user/useradd | ユーザーの作成
[**createObjectUsingPOST**](DefaultApi.md#createObjectUsingPOST) | **POST** /api/v1/user/objects | オブジェクトの作成
[**findAssetsUsingGET**](DefaultApi.md#findAssetsUsingGET) | **GET** /api/v1/user/assets/find | アセット検索
[**findCountObjectValuesUsingGET**](DefaultApi.md#findCountObjectValuesUsingGET) | **GET** /api/v1/user/objects/{objectId}/findCount | オブジェクトの登録データの検索結果件数
[**findObjectValuesUsingGET**](DefaultApi.md#findObjectValuesUsingGET) | **GET** /api/v1/user/objects/{objectId}/find | オブジェクトの登録データの検索
[**getObjectCountUsingGET**](DefaultApi.md#getObjectCountUsingGET) | **GET** /api/v1/user/objects/{objectId}/count | オブジェクトの登録件数の参照
[**getObjectValueUsingGET**](DefaultApi.md#getObjectValueUsingGET) | **GET** /api/v1/user/objects/{objectId}/{index} | オブジェクトの参照
[**getObjectValuesUsingGET**](DefaultApi.md#getObjectValuesUsingGET) | **GET** /api/v1/user/objects/{objectId} | オブジェクトの登録データの参照
[**queryAssetsBalanceUsingGET**](DefaultApi.md#queryAssetsBalanceUsingGET) | **GET** /api/v1/user/assets/{assetsName} | アセットの残高照会
[**queryAssetsTradingHistoryUsingGET**](DefaultApi.md#queryAssetsTradingHistoryUsingGET) | **GET** /api/v1/user/assets/{assetsName}/tradingHistory | アセットの取引履歴参照
[**sendAssetsUsingPOST**](DefaultApi.md#sendAssetsUsingPOST) | **POST** /api/v1/user/assets/{assetsName}/send | アセットの送信


# **addObjectValueUsingPOST**
> \Swagger\Client\Model\API_ addObjectValueUsingPOST($object_id, $object_value)

オブジェクトの登録

オブジェクトの登録を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトID
$object_value = new \Swagger\Client\Model\UserObjectValue(); // \Swagger\Client\Model\UserObjectValue | オブジェクト登録データ

try {
    $result = $api_instance->addObjectValueUsingPOST($object_id, $object_value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->addObjectValueUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトID |
 **object_value** | [**\Swagger\Client\Model\UserObjectValue**](../Model/\Swagger\Client\Model\UserObjectValue.md)| オブジェクト登録データ |

### Return type

[**\Swagger\Client\Model\API_**](../Model/API_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createAssetsUsingPOST**
> \Swagger\Client\Model\API_ createAssetsUsingPOST($assets)

アセット作成

アセットの作成を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$assets = new \Swagger\Client\Model\AssetsDetail(); // \Swagger\Client\Model\AssetsDetail | アセット作成情報

try {
    $result = $api_instance->createAssetsUsingPOST($assets);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createAssetsUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assets** | [**\Swagger\Client\Model\AssetsDetail**](../Model/\Swagger\Client\Model\AssetsDetail.md)| アセット作成情報 |

### Return type

[**\Swagger\Client\Model\API_**](../Model/API_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createNewAccountUsingPOST**
> \Swagger\Client\Model\_ createNewAccountUsingPOST($parameter)

ユーザーの作成

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$parameter = new \Swagger\Client\Model\_(); // \Swagger\Client\Model\_ | ユーザー情報

try {
    $result = $api_instance->createNewAccountUsingPOST($parameter);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createNewAccountUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parameter** | [**\Swagger\Client\Model\_**](../Model/\Swagger\Client\Model\_.md)| ユーザー情報 |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createObjectUsingPOST**
> \Swagger\Client\Model\API_ createObjectUsingPOST($user_object)

オブジェクトの作成

オブジェクトの作成を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$user_object = new \Swagger\Client\Model\ObjectDetail(); // \Swagger\Client\Model\ObjectDetail | オブジェクト作成情報

try {
    $result = $api_instance->createObjectUsingPOST($user_object);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createObjectUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_object** | [**\Swagger\Client\Model\ObjectDetail**](../Model/\Swagger\Client\Model\ObjectDetail.md)| オブジェクト作成情報 |

### Return type

[**\Swagger\Client\Model\API_**](../Model/API_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findAssetsUsingGET**
> \Swagger\Client\Model\_ findAssetsUsingGET($assets_name)

アセット検索

アセット名から登録されているアセットを検索します。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$assets_name = "assets_name_example"; // string | アセット名

try {
    $result = $api_instance->findAssetsUsingGET($assets_name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->findAssetsUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assets_name** | **string**| アセット名 |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findCountObjectValuesUsingGET**
> \Swagger\Client\Model\_ findCountObjectValuesUsingGET($object_id, $object_value)

オブジェクトの登録データの検索結果件数

登録されているオブジェクトのデータを中間一致で検索を行い該当件数を取得します。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトID
$object_value = "object_value_example"; // string | オブジェクト検索文字列

try {
    $result = $api_instance->findCountObjectValuesUsingGET($object_id, $object_value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->findCountObjectValuesUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトID |
 **object_value** | **string**| オブジェクト検索文字列 | [optional]

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findObjectValuesUsingGET**
> \Swagger\Client\Model\_ findObjectValuesUsingGET($object_id, $object_value)

オブジェクトの登録データの検索

登録されているオブジェクトのデータを中間一致で検索を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトID
$object_value = "object_value_example"; // string | オブジェクト検索文字列

try {
    $result = $api_instance->findObjectValuesUsingGET($object_id, $object_value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->findObjectValuesUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトID |
 **object_value** | **string**| オブジェクト検索文字列 | [optional]

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getObjectCountUsingGET**
> \Swagger\Client\Model\_ getObjectCountUsingGET($object_id)

オブジェクトの登録件数の参照

登録されているオブジェクトの件数を取得します。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトのキー

try {
    $result = $api_instance->getObjectCountUsingGET($object_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getObjectCountUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトのキー |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getObjectValueUsingGET**
> \Swagger\Client\Model\_ getObjectValueUsingGET($object_id, $index)

オブジェクトの参照

登録されているオブジェクトのインデックスによる参照を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトのキー
$index = 56; // int | オブジェクトのインデックス

try {
    $result = $api_instance->getObjectValueUsingGET($object_id, $index);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getObjectValueUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトのキー |
 **index** | **int**| オブジェクトのインデックス |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getObjectValuesUsingGET**
> \Swagger\Client\Model\_ getObjectValuesUsingGET($object_id)

オブジェクトの登録データの参照

登録されているオブジェクトのデータの一覧を取得します。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$object_id = "object_id_example"; // string | オブジェクトのキー

try {
    $result = $api_instance->getObjectValuesUsingGET($object_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getObjectValuesUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_id** | **string**| オブジェクトのキー |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **queryAssetsBalanceUsingGET**
> \Swagger\Client\Model\_ queryAssetsBalanceUsingGET($assets_name)

アセットの残高照会

アセットの残高照会を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$assets_name = "assets_name_example"; // string | アセット名

try {
    $result = $api_instance->queryAssetsBalanceUsingGET($assets_name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->queryAssetsBalanceUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assets_name** | **string**| アセット名 |

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **queryAssetsTradingHistoryUsingGET**
> \Swagger\Client\Model\_ queryAssetsTradingHistoryUsingGET($assets_name, $eth_address)

アセットの取引履歴参照

アセットの取引履歴明細の参照を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$assets_name = "assets_name_example"; // string | アセット名
$eth_address = "eth_address_example"; // string | ETHアドレス

try {
    $result = $api_instance->queryAssetsTradingHistoryUsingGET($assets_name, $eth_address);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->queryAssetsTradingHistoryUsingGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assets_name** | **string**| アセット名 |
 **eth_address** | **string**| ETHアドレス | [optional]

### Return type

[**\Swagger\Client\Model\_**](../Model/_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sendAssetsUsingPOST**
> \Swagger\Client\Model\API_ sendAssetsUsingPOST($assets_name, $send_assets)

アセットの送信

アセットの送信を行います。

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$assets_name = "assets_name_example"; // string | アセット名
$send_assets = new \Swagger\Client\Model\_(); // \Swagger\Client\Model\_ | アセット送信情報

try {
    $result = $api_instance->sendAssetsUsingPOST($assets_name, $send_assets);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sendAssetsUsingPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **assets_name** | **string**| アセット名 |
 **send_assets** | [**\Swagger\Client\Model\_**](../Model/\Swagger\Client\Model\_.md)| アセット送信情報 |

### Return type

[**\Swagger\Client\Model\API_**](../Model/API_.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: *_/_*

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

