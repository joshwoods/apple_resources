

- AudioDriverKit
- IOUserAudioCustomProperty
-  RemoveCustomProperty 

Instance Method

# RemoveCustomProperty

Attempts to remove a custom property from the custom property.

DriverKit 21.0+

``` source
kern_return_t RemoveCustomProperty(IOUserAudioCustomProperty * in_custom_property);
```

## Parameters 

`in_custom_property`  

An IOUserAudioCustomProperty object to remove from the IOUserAudioCustomProperty.

## Return Value

kIOReturnError

## Discussion

This method always returns kIOReturnError since a custom property can’t have a custom property.

## See Also

### Infrequently Used Functionality

AddCustomProperty

Attempts to add a custom property to the custom property.

