

- AudioDriverKit
- IOUserAudioBox
-  GetTransportType 

Instance Method

# GetTransportType

Returns the box’s transport type.

DriverKit 21.0+

``` source
IOUserAudioTransportType GetTransportType();
```

## Return Value

The audio box’s `IOUserAudioTransportType`.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Transport Types

SetTransportType

Sets the box’s transport type.

IOUserAudioTransportType

The type of transport to deliver audio.

