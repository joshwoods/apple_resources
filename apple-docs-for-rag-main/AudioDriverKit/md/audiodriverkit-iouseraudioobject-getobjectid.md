

- AudioDriverKit
- IOUserAudioObject
-  GetObjectID 

Instance Method

# GetObjectID

Gets the object’s identifier.

DriverKit 21.0+

``` source
IOUserAudioObjectID GetObjectID();
```

## Return Value

The object’s `IOUserAudioObjectID`.

## Discussion

Use this identifier when looking up a driver’s objects with GetAudioObjectForObjectID.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

IOUserAudioObjectID

An identifier that provides a handle on a specific audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

