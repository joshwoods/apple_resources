

- AudioDriverKit
- IOUserAudioDriver
-  GetBaseClassID 

Instance Method

# GetBaseClassID

Gets the audio class identifier of the base class object.

DriverKit 21.0+

``` source
IOUserAudioClassID GetBaseClassID();
```

## Return Value

The audio class identifier of the base class object.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

IOUserAudioClassID

An identifier for the type of audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

GetName

Gets the name of the driver.

SetName

Sets the name of the driver.

