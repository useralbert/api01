# openapi_client.DefaultApi

All URIs are relative to *http://localhost:3000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cites_from_state**](DefaultApi.md#get_cites_from_state) | **GET** /api/state/{stateId} | 
[**get_states**](DefaultApi.md#get_states) | **GET** /api/states | 


# **get_cites_from_state**
> list[str] get_cites_from_state(state_id)



Return a list of cities from the state

### Example

```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Create an instance of the API class
api_instance = openapi_client.DefaultApi()
state_id = openapi_client.State() # State | 

try:
    api_response = api_instance.get_cites_from_state(state_id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_cites_from_state: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **state_id** | [**State**](.md)|  | 

### Return type

**list[str]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: applications/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_states**
> State get_states()



Return a list of valid 2 character states

### Example

```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Create an instance of the API class
api_instance = openapi_client.DefaultApi()

try:
    api_response = api_instance.get_states()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_states: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**State**](State.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

