

- AudioDriverKit
- IOUserAudioCustomProperty
-  GetCustomPropertyValueWithQualifier 

Instance Method

# GetCustomPropertyValueWithQualifier

Gets the custom property value for a given qualifier.

DriverKit 21.0+

``` source
kern_return_t GetCustomPropertyValueWithQualifier(OSObject * in_qualifier_data, OSObject * * out_data);
```

## Parameters 

`in_qualifier_data`  

The property qualifier, as an OSObject. The caller retains and releases this object. This value is `NULL` if the qualifier data type is `CustomPropertyDataTypeNone`.

`out_data`  

On output, the property value, as an OSObject. The caller retains and releases this object.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Use this method to get the custom property’s data value, optionally adding a qualifier to further refine the action. For example, if a given property exists on multiple devices, use a device identifier as the qualifier to indicate which device to get the value from.

The base class returns the custom property value set on the object without looking at contents of the qualifier data. If the returned value should depend on the qualifier, subclass IOUserAudioCustomProperty and override this method.

## See Also

### Accessing the Data Value

SetQualifierAndDataValue

Sets the custom property’s data value.

GetCustomPropertyInfo

Gets a property info object that describes the custom property.

IOUserAudioCustomPropertyInfo

A description of a custom property’s data types.

