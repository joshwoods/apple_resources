

- AudioDriverKit
- IOUserAudioDriver
-  AddObject 

Instance Method

# AddObject

Adds an audio object to the driver.

DriverKit 21.0+

``` source
kern_return_t AddObject(IOUserAudioObject * in_object);
```

## Parameters 

`in_object`  

The IOUserAudioObjectID to add to the driver.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Use this method to add to the driver any objects that require management by the host. If the add succeeds, the object’s reference count increments by one. The caller should also call PropertiesChanged to notify the host of any changes.

## See Also

### Working with Audio Objects

RemoveObject

Removes an audio object from the driver.

GetAudioObjectForObjectID

Gets a pointer to an audio object, given the object’s identifier.

