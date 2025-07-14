

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBConfigurationDescHeader 

Type Alias

# IOUSBConfigurationDescHeader

The header of a configuration descriptor.

macOS 10.1+

``` source
typedef struct IOUSBConfigurationDescHeader IOUSBConfigurationDescHeader;
```

## Discussion

The header of a IOUSBConfigurationDescriptor that returns the total length of the descriptor.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

wTotalLength

The total length of the descriptor, including the length of all related interface, endpoint, and vendor-specific descriptors.

## See Also

### Configuration Descriptors

IOUSBConfigurationDescriptor

The structure for storing a USB configuration descriptor.

IOUSBConfigurationDescriptorPtr

A pointer to a configuration descriptor.

IOUSBConfigurationDescHeaderPtr

A pointer to a configuration descriptor header.

### Related Documentation

IOUSBConfigurationDescHeader

