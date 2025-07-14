

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioCustomPropertyInfo 

Structure

# IOUserAudioCustomPropertyInfo

A description of a custom property’s data types.

DriverKit 21.0+

``` source
struct IOUserAudioCustomPropertyInfo;
```

## Discussion

The description provided by the IOUserAudioCustomPropertyInfo structure allows the host to marshal the data between the host and its clients.

## Topics

### Property Metadata

mSelector

The property selector of the custom property.

mPropertyDataType

The data type of the of the custom property’s data.

mQualifierDataType

The data type of the of the custom property’s qualifier data.

## See Also

### Accessing the Data Value

SetQualifierAndDataValue

Sets the custom property’s data value.

GetCustomPropertyValueWithQualifier

Gets the custom property value for a given qualifier.

GetCustomPropertyInfo

Gets a property info object that describes the custom property.

