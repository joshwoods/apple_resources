

- AudioDriverKit
- IOUserAudioStream
-  StopIO 

Instance Method

# StopIO

Tells the stream to stop I/O.

DriverKit 21.0+

``` source
kern_return_t StopIO(IOUserAudioStartStopFlags in_flags);
```

## Parameters 

`in_flags`  

A `IOUserAudioStartStopFlag` to indicate I/O shutdown behavior.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation always returns kIOReturnSuccess.

Subclass and override this method to handle hardware-specific tasks during I/O shutdown, then call the superclass to update the I/O state. The framework expects this call to always succeed or fail.

## See Also

### Performing I/O

StartIO

Tells the stream to start I/O.

IOUserAudioStartStopFlags

Values that indicate I/O starts or stops.

