

- USBDriverKit
- IOUSBConfigurationDescriptor
-  MaxPower 

Instance Property

# MaxPower

The maximum power consumption of the USB device expressed in 2mA units.

DriverKit 19.0+

``` source
uint8_t MaxPower;
```

## Discussion

A value of 50 indicates that the device consumes a maximum of 100mA of current.

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

bConfigurationValue

The value to use when selecting this configuration.

iConfiguration

The index of the string descriptor that describes this configuration.

bmAttributes

A bitmask indicating the configuration’s characteristics.

