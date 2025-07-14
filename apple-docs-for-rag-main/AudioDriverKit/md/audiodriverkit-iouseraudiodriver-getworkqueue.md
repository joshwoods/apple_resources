

- AudioDriverKit
- IOUserAudioDriver
-  GetWorkQueue 

Instance Method

# GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

DriverKit 21.0+

``` source
OSSharedPtr GetWorkQueue();
```

## Return Value

The work queue created by the audio object.

## Discussion

The work queue synchronizes access to the driver’s state. Setters and getters for the driver do their work on the work queue.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

GetName

Gets the name of the driver.

SetName

Sets the name of the driver.

