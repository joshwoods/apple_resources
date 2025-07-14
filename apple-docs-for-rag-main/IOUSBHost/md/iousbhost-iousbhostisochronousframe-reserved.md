

- IOUSBHost
- IOUSBHostIsochronousFrame
-  reserved 

Instance Property

# reserved

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
var reserved: UInt32
```

## See Also

### Instance Properties

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var status: IOReturn

The completion status for an individual frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

