

- AudioDriverKit
- IOUserAudioDriver
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

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

GetName

Gets the name of the driver.

SetName

Sets the name of the driver.

