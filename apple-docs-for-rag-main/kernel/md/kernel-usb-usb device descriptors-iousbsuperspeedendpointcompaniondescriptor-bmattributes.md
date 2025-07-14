

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBSuperSpeedEndpointCompanionDescriptor
-  bmAttributes 

Instance Property

# bmAttributes

A bitmap encoding of supported device-level features.

macOS 10.7+

``` source
uint8_t bmAttributes;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bMaxBurst

The maximum number of packets the endpoint can send or receive as part of a burst.

wBytesPerInterval

The total number of bytes this endpoint transfers every service interval.

