

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDeviceQualifierDescriptor 

Type Alias

# IOUSBDeviceQualifierDescriptor

The structure for describing a high-speed capable USB device.

macOS 10.2+

``` source
typedef struct IOUSBDeviceQualifierDescriptor IOUSBDeviceQualifierDescriptor;
```

## Discussion

For information about this descriptor, see USB 2.0, 9.6.2.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bcdUSB

The USB specification version number.

bDeviceClass

The class code.

bDeviceSubClass

The subclass code.

bDeviceProtocol

The protocol code.

bMaxPacketSize0

The maximum packet size for other speed.

bNumConfigurations

The number of other-speed configurations.

bReserved

Reserved for future use.

## See Also

### Device Descriptors

IOUSBDeviceDescriptor

The structure for storing a USB device descriptor.

IOUSBDeviceDescriptorPtr

A pointer to a USB device descriptor.

IOUSBDeviceQualifierDescriptorPtr

A pointer to a qualifier descriptor.

### Related Documentation

IOUSBDeviceQualifierDescriptor

