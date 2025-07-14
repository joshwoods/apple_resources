

- AudioDriverKit
- IOUserAudioBox
-  SetTransportType 

Instance Method

# SetTransportType

Sets the box’s transport type.

DriverKit 21.0+

``` source
kern_return_t SetTransportType(IOUserAudioTransportType in_transport_type);
```

## Parameters 

`in_transport_type`  

The `IOUserAudioTransportType` to set for the audio box.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the transport type sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Transport Types

GetTransportType

Returns the box’s transport type.

IOUserAudioTransportType

The type of transport to deliver audio.

