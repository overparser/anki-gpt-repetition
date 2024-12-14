# PostUserRequest


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**telegram_login** | **str** |  | [optional] 
**telegram_id** | **int** |  | 
**registration_date** | **datetime** |  | [optional] [readonly] 
**username** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**last_updated** | **datetime** |  | [optional] 
**default_repeats** | **List[str]** |  | [optional] 
**preferences** | [**UserPreferences**](UserPreferences.md) |  | [optional] 
**last_update** | **datetime** |  | [optional] [readonly] 

## Example

```python
from openapi_client.models.post_user_request import PostUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PostUserRequest from a JSON string
post_user_request_instance = PostUserRequest.from_json(json)
# print the JSON string representation of the object
print PostUserRequest.to_json()

# convert the object into a dict
post_user_request_dict = post_user_request_instance.to_dict()
# create an instance of PostUserRequest from a dict
post_user_request_from_dict = PostUserRequest.from_dict(post_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


