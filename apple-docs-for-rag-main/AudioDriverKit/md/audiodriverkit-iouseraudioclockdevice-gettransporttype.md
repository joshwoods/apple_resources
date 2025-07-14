

- AudioDriverKit
- IOUserAudioClockDevice
-  GetTransportType 

Instance Method

# GetTransportType

Gets the transport type of the clock device.

DriverKit 21.0+

``` source
IOUserAudioTransportType GetTransportType();
```

## Return Value

The clock device’s transport type.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Transport Type

SetTransportType

Sets the transport type of the clock device.

IOUserAudioTransportType

The type of transport to deliver audio.

