

- IOUSBHost
- IOUSBHostIsochronousFrame
-  requestCount 

Instance Property

# requestCount

The number of requested bytes to transfer for the frame.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
var requestCount: UInt32
```

## Discussion

Important

Initialize this field before submitting the structure.

## See Also

### Frame Structure

var status: IOReturn

The completion status for an individual frame.

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

