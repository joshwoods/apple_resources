

- IOUSBHost
- IOUSBHostIsochronousFrame
-  completeCount 

Instance Property

# completeCount

The number of bytes that the system actually transferred for the frame.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
var completeCount: UInt32
```

## Discussion

IOUSBHost updates this field upon completion of the frame.

## See Also

### Frame Structure

var status: IOReturn

The completion status for an individual frame.

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

