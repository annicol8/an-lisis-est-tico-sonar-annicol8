# Solicitud


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cantidades_iniciales** | **List[int]** |  | [optional] 
**nombre_entidades** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.solicitud import Solicitud

# TODO update the JSON string below
json = "{}"
# create an instance of Solicitud from a JSON string
solicitud_instance = Solicitud.from_json(json)
# print the JSON string representation of the object
print Solicitud.to_json()

# convert the object into a dict
solicitud_dict = solicitud_instance.to_dict()
# create an instance of Solicitud from a dict
solicitud_form_dict = solicitud.from_dict(solicitud_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


