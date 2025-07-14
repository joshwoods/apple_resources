

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDFUDescriptor
-  bmAttributes 

Instance Property

# bmAttributes

A bitmap encoding of supported device-level features.

macOS 10.2+

``` source
uint8_t bmAttributes;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

wDetachTimeout

The time in milliseconds that the device waits after receipt of a detach request.

wTransferSize

The maximum number of bytes that the device can accept per control-write transaction.

