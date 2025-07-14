

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDescriptor 

Type Alias

# IOUSBDescriptor

The base descriptor type.

macOS 10.15+

``` source
typedef IOUSBDescriptorHeader IOUSBDescriptor;
```

## Discussion

Use this type to represent generic descriptor definitions. For more information about descriptors, see USB 3.2, 9.5.

## See Also

### Descriptor Fundamentals

IOUSBDescriptorHeader

The base descriptor header.

tIOUSBDescriptorType

Constants describing the types of descriptors available for a USB device.

tIOUSBDescriptorSize

Constants for the number of bytes in descriptor structures.

IOUSBDescriptorHeaderPtr

A pointer to a USB descriptor header.

