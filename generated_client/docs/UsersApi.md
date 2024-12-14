# openapi_client.UsersApi

All URIs are relative to *http://localhost:8001*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_users_user_id**](UsersApi.md#delete_users_user_id) | **DELETE** /users/{userId} | Delete User
[**get_users_user_id**](UsersApi.md#get_users_user_id) | **GET** /users/{userId} | Get User Info by User ID
[**patch_users_user_id**](UsersApi.md#patch_users_user_id) | **PATCH** /users/{userId} | Update User Information
[**post_user**](UsersApi.md#post_user) | **POST** /user | Create New User


# **delete_users_user_id**
> User delete_users_user_id(user_id)

Delete User

Delete an existing user.

### Example

```python
import time
import os
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8001
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:8001"
)


# Enter a context with an instance of the API client
async with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.UsersApi(api_client)
    user_id = 'user_id_example' # str | user id

    try:
        # Delete User
        api_response = await api_instance.delete_users_user_id(user_id)
        print("The response of UsersApi->delete_users_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->delete_users_user_id: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**| user id | 

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | User Deleted |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_users_user_id**
> User get_users_user_id(user_id)

Get User Info by User ID

Retrieve the information of the user with the matching user ID.

### Example

```python
import time
import os
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8001
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:8001"
)


# Enter a context with an instance of the API client
async with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.UsersApi(api_client)
    user_id = 'user_id_example' # str | user id

    try:
        # Get User Info by User ID
        api_response = await api_instance.get_users_user_id(user_id)
        print("The response of UsersApi->get_users_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->get_users_user_id: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**| user id | 

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | User Found |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_users_user_id**
> User patch_users_user_id(user_id, patch_users_user_id_request=patch_users_user_id_request)

Update User Information

Update the information of an existing user.

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.patch_users_user_id_request import PatchUsersUserIdRequest
from openapi_client.models.user import User
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8001
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:8001"
)


# Enter a context with an instance of the API client
async with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.UsersApi(api_client)
    user_id = 'user_id_example' # str | user id
    patch_users_user_id_request = openapi_client.PatchUsersUserIdRequest() # PatchUsersUserIdRequest | Update user information (optional)

    try:
        # Update User Information
        api_response = await api_instance.patch_users_user_id(user_id, patch_users_user_id_request=patch_users_user_id_request)
        print("The response of UsersApi->patch_users_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->patch_users_user_id: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**| user id | 
 **patch_users_user_id_request** | [**PatchUsersUserIdRequest**](PatchUsersUserIdRequest.md)| Update user information | [optional] 

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | User Updated |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_user**
> User post_user(post_user_request=post_user_request)

Create New User

Create a new user.

### Example

```python
import time
import os
import openapi_client
from openapi_client.models.post_user_request import PostUserRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8001
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:8001"
)


# Enter a context with an instance of the API client
async with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.UsersApi(api_client)
    post_user_request = {"user_id":"string","telegram_login":"string","telegram_id":6453843256,"registration_date":"2019-08-24T14:15:22Z","username":"string","status":"active","last_updated":"2019-08-24T14:15:22Z","default_repeats":["300 seconds"],"preferences":{"language":"string"}} # PostUserRequest |  (optional)

    try:
        # Create New User
        api_response = await api_instance.post_user(post_user_request=post_user_request)
        print("The response of UsersApi->post_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->post_user: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_user_request** | [**PostUserRequest**](PostUserRequest.md)|  | [optional] 

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Shared Response |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

