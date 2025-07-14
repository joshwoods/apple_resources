

- USBDriverKit
- IOUSBConfigurationDescriptor
-  wTotalLength 

Instance Property

# wTotalLength

The total length of the descriptor, including the length of all related interface, endpoint, and vendor-specific descriptors.

DriverKit 19.0+

``` source
uint16_t wTotalLength;
```

## See Also

### Getting the Descriptor Properties

bLength

The size of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bNumInterfaces

The number of interfaces this configuration supports.

bConfigurationValue

The value to use when selecting this configuration.

iConfiguration

The index of the string descriptor that describes this configuration.

bmAttributes

A bitmask indicating the configuration’s characteristics.

MaxPower

The maximum power consumption of the USB device expressed in 2mA units.

