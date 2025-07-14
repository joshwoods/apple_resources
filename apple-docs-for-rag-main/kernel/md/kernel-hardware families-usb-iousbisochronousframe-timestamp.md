

- Kernel
- Hardware Families
- USB
- IOUSBIsochronousFrame
-  timeStamp 

Instance Property

# timeStamp

The frame’s observed completion time.

macOS 10.15+

``` source
uint64_t timeStamp;
```

## Discussion

Interrupt latency and system load may result in more than one frame completing with the same timestamp.

## See Also

### Getting the Frame Properties

status

The completion status for this individual frame.

requestCount

The number of bytes to transfer for this frame.

completeCount

The number of bytes that the system actually transferred for this frame.

reserved

Reserved for future use.

