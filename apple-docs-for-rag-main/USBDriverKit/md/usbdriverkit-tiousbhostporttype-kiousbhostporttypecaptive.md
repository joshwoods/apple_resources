

- USBDriverKit
- tIOUSBHostPortType
-  kIOUSBHostPortTypeCaptive 

Enumeration Case

# kIOUSBHostPortTypeCaptive

A port for which the device cannot be physically disconnected.

DriverKit 19.0+

``` source
kIOUSBHostPortTypeCaptive
```

## See Also

### Getting the Port Types

kIOUSBHostPortTypeStandard

A general-purpose USB port.

kIOUSBHostPortTypeInternal

A port that cannot be physically disconnected from the host machine.

kIOUSBHostPortTypeAccessory

A port for which the device might require additional authentication before a driver can access it.

kIOUSBHostPortTypeExpressCard

A port containing an expansion card.

kIOUSBHostPortTypeCount

The number of port types.

