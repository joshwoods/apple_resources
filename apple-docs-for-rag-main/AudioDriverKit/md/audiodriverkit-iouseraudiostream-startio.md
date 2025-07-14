

- AudioDriverKit
- IOUserAudioStream
-  StartIO 

Instance Method

# StartIO

Tells the stream to start I/O.

DriverKit 21.0+

``` source
kern_return_t StartIO(IOUserAudioStartStopFlags in_flags);
```

## Parameters 

`in_flags`  

A `IOUserAudioStartStopFlag` to indicate I/O startup behavior.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation always returns kIOReturnSuccess.

Subclass and override this method to handle hardware-specific tasks during I/O startup, then call the superclass to update the I/O state. The framework expects this call to always succeed or fail. The hardware can take as long as it needs in this call, provided it always either succeeds or fails.

## See Also

### Performing I/O

StopIO

Tells the stream to stop I/O.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

