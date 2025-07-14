

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDFUDescriptor 

Type Alias

# IOUSBDFUDescriptor

A structure that defines the USB device firmware update descriptor.

macOS 10.2+

``` source
typedef struct IOUSBDFUDescriptor IOUSBDFUDescriptor;
```

## Discussion

See the USB Implementers Forum (USB-IF) *Universal Serial Bus Power Delivery Firmware Update Specification* for more information.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bmAttributes

A bitmap encoding of supported device-level features.

wDetachTimeout

The time in milliseconds that the device waits after receipt of a detach request.

wTransferSize

The maximum number of bytes that the device can accept per control-write transaction.

## See Also

### Device Firmware Update Descriptors

IOUSBDFUDescriptorPtr

A pointer to a structure that defines the USB device firmware update descriptor.

### Related Documentation

IOUSBDFUDescriptor

