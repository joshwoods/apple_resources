

- AudioDriverKit
- IOUserAudioDriver
-  GetName 

Instance Method

# GetName

Gets the name of the driver.

DriverKit 21.0+

``` source
OSSharedPtr GetName();
```

## Return Value

A `OSSharedPtr` to an OSString containing the driver name.

## Discussion

Getting the name synchronizes by using the work queue created by the object.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

GetBaseClassID

Gets the audio class identifier of the base class object.

IOUserAudioClassID

An identifier for the type of audio object.

GetWorkQueue

Gets the work queue created by the audio object, as a pointer to a dispatch queue.

SetName

Sets the name of the driver.

