

- IOUSBHost
- IOUSBHostIsochronousFrame
-  timeStamp 

Instance Property

# timeStamp

The observed time for the frame’s completion.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
var timeStamp: IOUSBHostTime
```

## Discussion

Note

Interrupt latency and system load may result in more than one frame completing with the same timestamp.

## See Also

### Frame Structure

var status: IOReturn

The completion status for an individual frame.

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

