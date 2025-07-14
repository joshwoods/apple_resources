

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBConfigurationDescriptor 

Type Alias

# IOUSBConfigurationDescriptor

The structure for storing a USB configuration descriptor.

macOS 10.0+

``` source
typedef struct IOUSBConfigurationDescriptor IOUSBConfigurationDescriptor;
```

## Discussion

This descriptor contains information about a specific configuration of a device, including the interfaces that configuration provides. This structure has a variable length so it defines only the known fields. Use the `wTotalLength` field to read the entire descriptor.

For more information about this descriptor type, see USB 3.2, 9.6.3.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

wTotalLength

The total length of the descriptor, including the length of all related interface, endpoint, and vendor-specific descriptors.

bNumInterfaces

The number of interfaces this configuration supports.

bConfigurationValue

The value to use when selecting this configuration.

iConfiguration

The index of the string descriptor that describes this configuration.

bmAttributes

A bit mask indicating the configuration’s characteristics.

MaxPower

The maximum power consumption of the USB device expressed in 2 milliamp units.

## See Also

### Configuration Descriptors

IOUSBConfigurationDescHeader

The header of a configuration descriptor.

IOUSBConfigurationDescriptorPtr

A pointer to a configuration descriptor.

IOUSBConfigurationDescHeaderPtr

A pointer to a configuration descriptor header.

### Related Documentation

IOUSBConfigurationDescriptor

