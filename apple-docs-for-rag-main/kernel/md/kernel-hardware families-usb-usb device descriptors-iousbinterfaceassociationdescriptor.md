

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBInterfaceAssociationDescriptor 

Type Alias

# IOUSBInterfaceAssociationDescriptor

The descriptor that associates multiple interfaces to the same function.

macOS 10.3+

``` source
typedef struct IOUSBInterfaceAssociationDescriptor IOUSBInterfaceAssociationDescriptor;
```

## Discussion

See USB 3.2, 9.6.4 for more information.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bFirstInterface

The first interface of the descriptor.

bInterfaceCount

The number of interfaces.

bFunctionClass

The function class.

bFunctionSubClass

The function subclass.

bFunctionProtocol

The function protocol.

iFunction

The descriptor’s function.

## See Also

### Interface Descriptors

IOUSBInterfaceDescriptor

A descriptor for a specific interface of a USB device.

IOUSBInterfaceDescriptorPtr

A pointer to a USB interface descriptor.

IOUSBInterfaceAssociationDescriptorPtr

A pointer to a USB interface association descriptor.

### Related Documentation

IOUSBInterfaceAssociationDescriptor

