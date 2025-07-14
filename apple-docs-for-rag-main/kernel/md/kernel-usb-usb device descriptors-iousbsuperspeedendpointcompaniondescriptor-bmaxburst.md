

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBSuperSpeedEndpointCompanionDescriptor
-  bMaxBurst 

Instance Property

# bMaxBurst

The maximum number of packets the endpoint can send or receive as part of a burst.

macOS 10.7+

``` source
uint8_t bMaxBurst;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bmAttributes

A bitmap encoding of supported device-level features.

wBytesPerInterval

The total number of bytes this endpoint transfers every service interval.

