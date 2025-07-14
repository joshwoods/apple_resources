

- AudioDriverKit
- IOUserAudioDriver
-  SetTransportType 

Instance Method

# SetTransportType

Set the transport type of the driver.

DriverKit 21.0+

``` source
kern_return_t SetTransportType(IOUserAudioTransportType in_transport_type);
```

## Parameters 

`in_transport_type`  

The audio transport type to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

You can change the transport type dynamically. If the change succeeds, the framework sends a notification to the host to update its object state.

## See Also

### Working with Transport Type

GetTransportType

Gets the transport type of the driver.

IOUserAudioTransportType

The type of transport to deliver audio.

