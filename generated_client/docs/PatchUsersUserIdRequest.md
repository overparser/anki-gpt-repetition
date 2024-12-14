# PatchUsersUserIdRequest


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**telegram_login** | **str** |  | [optional] 
**telegram_id** | **int** |  | [optional] 
**registration_date** | **datetime** |  | [optional] [readonly] 
**username** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**last_updated** | **datetime** |  | [optional] 
**default_repeats** | **List[str]** |  | [optional] 
**preferences** | [**UserPreferences**](UserPreferences.md) |  | [optional] 
**last_update** | **datetime** |  | [optional] [readonly] 

## Example

```python
from openapi_client.models.patch_users_user_id_request import PatchUsersUserIdRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PatchUsersUserIdRequest from a JSON string
patch_users_user_id_request_instance = PatchUsersUserIdRequest.from_json(json)
# print the JSON string representation of the object
print PatchUsersUserIdRequest.to_json()

# convert the object into a dict
patch_users_user_id_request_dict = patch_users_user_id_request_instance.to_dict()
# create an instance of PatchUsersUserIdRequest from a dict
patch_users_user_id_request_from_dict = PatchUsersUserIdRequest.from_dict(patch_users_user_id_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


