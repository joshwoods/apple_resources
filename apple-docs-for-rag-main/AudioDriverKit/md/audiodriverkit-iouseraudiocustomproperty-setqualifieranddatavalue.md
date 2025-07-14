

- AudioDriverKit
- IOUserAudioCustomProperty
-  SetQualifierAndDataValue 

Instance Method

# SetQualifierAndDataValue

Sets the custom property’s data value.

DriverKit 21.0+

``` source
kern_return_t SetQualifierAndDataValue(OSObject * in_qualifier_data, OSObject * in_data);
```

## Parameters 

`in_qualifier_data`  

The qualifier data for the custom property that corresponds to the data value. The type of this parameter must match the qualifier data type originally used for initializing the property. If the qualifier data type is `IOUserAudioCustomPropertyDataType::None`, this parameter must be `NULL`. If the qualifier data type is String, this parameter must be an OSString. If the qualifier data type is Dictionary, this parameter must be an OSDictionary.

`in_data`  

The data object for the custom property that corresponds to the qualifier. The type of this parameter must match the data type originally used for initializing the property. If the data type is String, this parameter must be an OSString. If the qualifier data type is Dictionary, this parameter must be an OSDictionary. This parameter can’t be `NULL`.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Use this method to set the custom property’s data value, optionally adding a qualifier to further refine the action. For example, if a given property exists on multiple devices, use a device identifier as the qualifier to indicate which device to set the value on.

## See Also

### Accessing the Data Value

GetCustomPropertyValueWithQualifier

Gets the custom property value for a given qualifier.

GetCustomPropertyInfo

Gets a property info object that describes the custom property.

IOUserAudioCustomPropertyInfo

A description of a custom property’s data types.

