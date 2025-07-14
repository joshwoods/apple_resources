

- AudioDriverKit
- IOUserAudioObject
-  GetClassID 

Instance Method

# GetClassID

Gets the audio class identifier of the object.

DriverKit 21.0+

``` source
IOUserAudioClassID GetClassID();
```

## Return Value

The audio class identifier of the object.

## See Also

### Getting Information About the Class

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

GetObjectID

Gets the object’s identifier.

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

