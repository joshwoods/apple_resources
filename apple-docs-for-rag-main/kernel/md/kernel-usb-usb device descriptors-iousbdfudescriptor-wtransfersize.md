

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDFUDescriptor
-  wTransferSize 

Instance Property

# wTransferSize

The maximum number of bytes that the device can accept per control-write transaction.

macOS 10.2+

``` source
uint16_t wTransferSize;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bmAttributes

A bitmap encoding of supported device-level features.

wDetachTimeout

The time in milliseconds that the device waits after receipt of a detach request.

