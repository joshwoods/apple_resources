

- AudioDriverKit
- IOUserAudioClockDevice
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

## Discussion

This method overrides the base class IOUserAudioObject.

## See Also

### Getting Information About the Class

GetClassID

Gets the audio class identifier of the object.

IOUserAudioClassID

An identifier for the type of audio object.

