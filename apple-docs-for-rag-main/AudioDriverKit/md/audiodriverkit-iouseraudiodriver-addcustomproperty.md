

- AudioDriverKit
- IOUserAudioDriver
-  AddCustomProperty 

Instance Method

# AddCustomProperty

Adds a custom property object to the driver.

DriverKit 21.0+

``` source
kern_return_t AddCustomProperty(IOUserAudioCustomProperty * in_custom_property);
```

## Parameters 

`in_custom_property`  

An IOUserAudioCustomProperty object to add to the IOUserAudioDriver.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Working with Custom Properties

RemoveCustomProperty

Removes a previously-added custom property object from the driver.

IOUserAudioCustomProperty

A custom property to associate with audio objects.

