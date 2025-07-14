

- Kernel
- Hardware Families
- USB
- IOUSBIsochronousFrame
-  completeCount 

Instance Property

# completeCount

The number of bytes that the system actually transferred for this frame.

macOS 10.15+

``` source
uint32_t completeCount;
```

## Discussion

The system updates this field upon completion of the frame.

## See Also

### Getting the Frame Properties

status

The completion status for this individual frame.

requestCount

The number of bytes to transfer for this frame.

reserved

Reserved for future use.

timeStamp

The frame’s observed completion time.

