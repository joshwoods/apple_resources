

- USBDriverKit
-  tIOUSBHostPortType 

Enumeration

# tIOUSBHostPortType

Constants indicating a port’s type.

DriverKit 19.0+

``` source
enum tIOUSBHostPortType : unsigned int;
```

## Topics

### Getting the Port Types

kIOUSBHostPortTypeStandard

A general-purpose USB port.

kIOUSBHostPortTypeCaptive

A port for which the device cannot be physically disconnected.

kIOUSBHostPortTypeInternal

A port that cannot be physically disconnected from the host machine.

kIOUSBHostPortTypeAccessory

A port for which the device might require additional authentication before a driver can access it.

kIOUSBHostPortTypeExpressCard

A port containing an expansion card.

kIOUSBHostPortTypeCount

The number of port types.

## See Also

### Getting Device Information

GetAddress

Returns the address of the device.

GetSpeed

Retrieves the device’s operational speed.

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Returns the current port status of the device.

tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

tIOUSBHostPortStatus

Constants indicating the state of a port.

