

- USBDriverKit
- IOUSBIsochronousFrame
-  requestCount 

Instance Property

# requestCount

The number of bytes to transfer for this frame.

DriverKit 19.0+

``` source
uint32_t requestCount;
```

## Discussion

Set the value of this field before making an isochronous request.

## See Also

### Getting the Frame Properties

status

The completion status for this individual frame.

completeCount

The number of bytes actually transferred for this frame.

reserved

Reserved for future use.

timeStamp

The frame’s observed completion time.

