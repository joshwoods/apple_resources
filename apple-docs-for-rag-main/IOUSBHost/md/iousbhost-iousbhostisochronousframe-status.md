

- IOUSBHost
- IOUSBHostIsochronousFrame
-  status 

Instance Property

# status

The completion status for an individual frame.

Mac Catalyst 14.0+macOS 10.15–11.0Deprecated

``` source
var status: IOReturn
```

## Discussion

IOUSBHost initializes this to kIOReturnInvalid and updates the field with a valid status code upon completion of the frame.

## See Also

### Frame Structure

var requestCount: UInt32

The number of requested bytes to transfer for the frame.

var completeCount: UInt32

The number of bytes that the system actually transferred for the frame.

var timeStamp: IOUSBHostTime

The observed time for the frame’s completion.

