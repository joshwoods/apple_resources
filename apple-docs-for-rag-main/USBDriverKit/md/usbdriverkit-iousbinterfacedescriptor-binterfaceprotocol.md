

- USBDriverKit
- IOUSBInterfaceDescriptor
-  bInterfaceProtocol 

Instance Property

# bInterfaceProtocol

The protocol that this interface supports.

DriverKit 19.0+

``` source
uint8_t bInterfaceProtocol;
```

## See Also

### Accessing the Descriptor Properties

bLength

The size of this descriptor in bytes.

bDescriptorType

A constant value indicating an interface descriptor.

bInterfaceNumber

The zero-based index of this interface in the current configuration.

bAlternateSetting

The alternative setting for the interface.

bNumEndpoints

The number of endpoints that this interface uses.

bInterfaceClass

The class code indicating the behavior of this interface.

bInterfaceSubClass

The subclass code that further defines the behavior of this interface.

iInterface

The index of a string descriptor that describes this interface.

