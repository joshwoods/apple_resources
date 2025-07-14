

- USBDriverKit
- IOUSBIsochronousFrame
-  status 

Instance Property

# status

The completion status for this individual frame.

DriverKit 19.0+

``` source
IOReturn status;
```

## Discussion

The system initializes this field to `kIOReturnInvalid` and updates it with a valid status code upon completion of the frame.

## See Also

### Getting the Frame Properties

requestCount

The number of bytes to transfer for this frame.

completeCount

The number of bytes actually transferred for this frame.

reserved

Reserved for future use.

timeStamp

The frame’s observed completion time.

