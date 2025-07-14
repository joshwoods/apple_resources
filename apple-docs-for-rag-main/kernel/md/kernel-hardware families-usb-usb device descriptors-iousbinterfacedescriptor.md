

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBInterfaceDescriptor 

Type Alias

# IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

macOS 10.0+

``` source
typedef struct IOUSBInterfaceDescriptor IOUSBInterfaceDescriptor;
```

## Discussion

An `IOUSBInterfaceDescriptor` object contains information about one of the device’s supported interfaces. A device’s configuration provides one or more interfaces, each with zero or more endpoints that define how to configure the pipes for that device.

For more information about this descriptor type, see USB 3.2, 9.6.5.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bInterfaceNumber

The number of this interface.

bAlternateSetting

The value for selecting an alternative setting for the interface that the interface number references.

bNumEndpoints

The number of endpoints that the interface uses.

bInterfaceClass

The class code.

bInterfaceSubClass

The subclass code.

bInterfaceProtocol

The protocol code.

iInterface

The index of the string descriptor describing this interface.

## See Also

### Interface Descriptors

IOUSBInterfaceDescriptorPtr

A pointer to a USB interface descriptor.

IOUSBInterfaceAssociationDescriptor

The descriptor that associates multiple interfaces to the same function.

IOUSBInterfaceAssociationDescriptorPtr

A pointer to a USB interface association descriptor.

### Related Documentation

IOUSBInterfaceDescriptor

