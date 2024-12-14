# GetUsersUserId404ResponseError


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | [optional] 
**message** | **str** |  | [optional] 
**details** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.get_users_user_id404_response_error import GetUsersUserId404ResponseError

# TODO update the JSON string below
json = "{}"
# create an instance of GetUsersUserId404ResponseError from a JSON string
get_users_user_id404_response_error_instance = GetUsersUserId404ResponseError.from_json(json)
# print the JSON string representation of the object
print GetUsersUserId404ResponseError.to_json()

# convert the object into a dict
get_users_user_id404_response_error_dict = get_users_user_id404_response_error_instance.to_dict()
# create an instance of GetUsersUserId404ResponseError from a dict
get_users_user_id404_response_error_from_dict = GetUsersUserId404ResponseError.from_dict(get_users_user_id404_response_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


