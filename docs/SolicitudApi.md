# openapi_client.SolicitudApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**solicitud_comprobar_solicitud_get**](SolicitudApi.md#solicitud_comprobar_solicitud_get) | **GET** /Solicitud/ComprobarSolicitud | 
[**solicitud_get_solicitudes_usuario_get**](SolicitudApi.md#solicitud_get_solicitudes_usuario_get) | **GET** /Solicitud/GetSolicitudesUsuario | 
[**solicitud_solicitar_post**](SolicitudApi.md#solicitud_solicitar_post) | **POST** /Solicitud/Solicitar | 


# **solicitud_comprobar_solicitud_get**
> List[int] solicitud_comprobar_solicitud_get(nombre_usuario=nombre_usuario, tok=tok)



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
    api_instance = openapi_client.SolicitudApi(api_client)
    nombre_usuario = 'nombre_usuario_example' # str |  (optional)
    tok = 56 # int |  (optional)

    try:
        api_response = api_instance.solicitud_comprobar_solicitud_get(nombre_usuario=nombre_usuario, tok=tok)
        print("The response of SolicitudApi->solicitud_comprobar_solicitud_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolicitudApi->solicitud_comprobar_solicitud_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nombre_usuario** | **str**|  | [optional] 
 **tok** | **int**|  | [optional] 

### Return type

**List[int]**

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

# **solicitud_get_solicitudes_usuario_get**
> List[int] solicitud_get_solicitudes_usuario_get(nombre_usuario=nombre_usuario)



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
    api_instance = openapi_client.SolicitudApi(api_client)
    nombre_usuario = 'nombre_usuario_example' # str |  (optional)

    try:
        api_response = api_instance.solicitud_get_solicitudes_usuario_get(nombre_usuario=nombre_usuario)
        print("The response of SolicitudApi->solicitud_get_solicitudes_usuario_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolicitudApi->solicitud_get_solicitudes_usuario_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nombre_usuario** | **str**|  | [optional] 

### Return type

**List[int]**

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

# **solicitud_solicitar_post**
> object solicitud_solicitar_post(nombre_usuario=nombre_usuario, solicitud=solicitud)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.solicitud import Solicitud
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
    api_instance = openapi_client.SolicitudApi(api_client)
    nombre_usuario = 'nombre_usuario_example' # str |  (optional)
    solicitud = openapi_client.Solicitud() # Solicitud |  (optional)

    try:
        api_response = api_instance.solicitud_solicitar_post(nombre_usuario=nombre_usuario, solicitud=solicitud)
        print("The response of SolicitudApi->solicitud_solicitar_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolicitudApi->solicitud_solicitar_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nombre_usuario** | **str**|  | [optional] 
 **solicitud** | [**Solicitud**](Solicitud.md)|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

