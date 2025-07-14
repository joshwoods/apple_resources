

- AudioDriverKit
- IOUserAudioCustomProperty
-  HandleChangeCustomPropertyDataValueWithQualifier 

Instance Method

# HandleChangeCustomPropertyDataValueWithQualifier

Tells the property the data value is changing.

DriverKit 21.0+

``` source
kern_return_t HandleChangeCustomPropertyDataValueWithQualifier(OSObject * in_qualifier_data, OSObject * in_data);
```

## Parameters 

`in_qualifier_data`  

The qualifier data OSObject associated with setting the property data value. This can be an OSString, OSDictionary, or `NULL`.

`in_data`  

An OSObject to set as the custom property value.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation sets the value and returns kIOReturnSuccess, without checking the qualifier data. Subclass and override this method to handle changes to the custom property and return kIOReturnSuccess upon success.

