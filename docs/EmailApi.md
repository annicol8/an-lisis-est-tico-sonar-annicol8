# openapi_client.EmailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**email_post**](EmailApi.md#email_post) | **POST** /Email | 


# **email_post**
> EmailResponse email_post(email_address=email_address, message=message)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.email_response import EmailResponse
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
    api_instance = openapi_client.EmailApi(api_client)
    email_address = 'email_address_example' # str |  (optional)
    message = 'message_example' # str |  (optional)

    try:
        api_response = api_instance.email_post(email_address=email_address, message=message)
        print("The response of EmailApi->email_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailApi->email_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address** | **str**|  | [optional] 
 **message** | **str**|  | [optional] 

### Return type

[**EmailResponse**](EmailResponse.md)

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

