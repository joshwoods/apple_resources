

- AudioDriverKit
- IOUserAudioClockDevice
-  SetTransportType 

Instance Method

# SetTransportType

Sets the transport type of the clock device.

DriverKit 21.0+

``` source
kern_return_t SetTransportType(IOUserAudioTransportType in_transport_type);
```

## Parameters 

`in_transport_type`  

The transport type to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Drivers can change the transport type of the clock device dynamically. If successful, changing the transport type sends a notification to the host to update the object state.

## See Also

### Working with Transport Type

GetTransportType

Gets the transport type of the clock device.

IOUserAudioTransportType

The type of transport to deliver audio.

