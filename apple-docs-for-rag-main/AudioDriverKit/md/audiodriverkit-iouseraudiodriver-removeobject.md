

- AudioDriverKit
- IOUserAudioDriver
-  RemoveObject 

Instance Method

# RemoveObject

Removes an audio object from the driver.

DriverKit 21.0+

``` source
kern_return_t RemoveObject(IOUserAudioObject * in_object);
```

## Parameters 

`in_object`  

The IOUserAudioObjectID to remove from the driver.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If the remove succeeds, the object’s reference count decrements by one. The caller should also call PropertiesChanged to notify the host of any changes.

## See Also

### Working with Audio Objects

AddObject

Adds an audio object to the driver.

GetAudioObjectForObjectID

Gets a pointer to an audio object, given the object’s identifier.

