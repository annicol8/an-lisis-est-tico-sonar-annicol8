# openapi_client.ResultadosApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resultados_post**](ResultadosApi.md#resultados_post) | **POST** /Resultados | 


# **resultados_post**
> object resultados_post(nombre_usuario=nombre_usuario, tok=tok)



### Example

```python
import time
import os
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.ResultadosApi(api_client)
    nombre_usuario = 'nombre_usuario_example' # str |  (optional)
    tok = 56 # int |  (optional)

    try:
        api_response = api_instance.resultados_post(nombre_usuario=nombre_usuario, tok=tok)
        print("The response of ResultadosApi->resultados_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResultadosApi->resultados_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nombre_usuario** | **str**|  | [optional] 
 **tok** | **int**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

