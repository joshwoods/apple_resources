

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDescriptorHeader 

Type Alias

# IOUSBDescriptorHeader

The base descriptor header.

macOS 10.0+

``` source
typedef struct IOUSBDescriptorHeader IOUSBDescriptorHeader;
```

## Discussion

This structure is the standard header for all USB descriptors. Use it to read the length of a descriptor so that it can allocate storage for the whole descriptor.

## Topics

### Getting the Descriptor Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

## See Also

### Descriptor Fundamentals

IOUSBDescriptor

The base descriptor type.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

IOUSBDescriptorHeaderPtr

A pointer to a USB descriptor header.

### Related Documentation

IOUSBDescriptorHeader

