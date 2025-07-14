

- USBDriverKit
- IOUSBConfigurationDescriptor
-  bConfigurationValue 

Instance Property

# bConfigurationValue

The value to use when selecting this configuration.

DriverKit 19.0+

``` source
uint8_t bConfigurationValue;
```

## See Also

### Getting the Descriptor Properties

bLength

The size of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

wTotalLength

The total length of the descriptor, including the length of all related interface, endpoint, and vendor-specific descriptors.

bNumInterfaces

The number of interfaces this configuration supports.

iConfiguration

The index of the string descriptor that describes this configuration.

bmAttributes

A bitmask indicating the configuration’s characteristics.

MaxPower

The maximum power consumption of the USB device expressed in 2mA units.

