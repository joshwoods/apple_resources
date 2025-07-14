

- AudioDriverKit
- IOUserAudioObject
-  RemoveCustomProperty 

Instance Method

# RemoveCustomProperty

Removes a previously-added custom property object from the audio object.

DriverKit 21.0+

``` source
kern_return_t RemoveCustomProperty(IOUserAudioCustomProperty * in_custom_property);
```

## Parameters 

`in_custom_property`  

An IOUserAudioCustomProperty object to remove from the IOUserAudioObject.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Using Custom Properties

AddCustomProperty

Adds a custom property to the audio object.

IOUserAudioCustomProperty

A custom property to associate with audio objects.

