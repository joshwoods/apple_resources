

- AudioDriverKit
- IOUserAudioDriver
-  GetAudioObjectForObjectID 

Instance Method

# GetAudioObjectForObjectID

Gets a pointer to an audio object, given the object’s identifier.

DriverKit 21.0+

``` source
OSSharedPtr GetAudioObjectForObjectID(IOUserAudioObjectID in_object_id);
```

## Parameters 

`in_object_id`  

The IOUserAudioObjectID of an object previously added to the driver.

## Return Value

An `OSSharedPtr` to an IOUserAudioObject if `in_object_id` was found.

## See Also

### Working with Audio Objects

AddObject

Adds an audio object to the driver.

RemoveObject

Removes an audio object from the driver.

