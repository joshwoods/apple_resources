

- AudioDriverKit
- IOUserAudioDriver
-  GetTransportType 

Instance Method

# GetTransportType

Gets the transport type of the driver.

DriverKit 21.0+

``` source
IOUserAudioTransportType GetTransportType();
```

## Return Value

The transport type of the driver.

## Discussion

Getting the value synchronizes by using the work queue created by the object.

## See Also

### Working with Transport Type

SetTransportType

Set the transport type of the driver.

IOUserAudioTransportType

The type of transport to deliver audio.

