

- USBDriverKit
-  tIOUSBHostConnectionSpeed 

Enumeration

# tIOUSBHostConnectionSpeed

Constants indicating the connection speed of the device.

DriverKit 19.0+

``` source
enum tIOUSBHostConnectionSpeed : unsigned int;
```

## Discussion

This enumeration matches the default speed ID mappings defined in XHCI 1.0 Table 147.

## Topics

### Getting the Connection Speeds

kIOUSBHostConnectionSpeedNone

No device is connected.

kIOUSBHostConnectionSpeedFull

The connected device runs at 12 megabits per second.

kIOUSBHostConnectionSpeedLow

The connected device runs at 1.5 megabits per second.

kIOUSBHostConnectionSpeedHigh

The connected device runs at 480 megabits per second.

kIOUSBHostConnectionSpeedSuper

The connected device runs at 5 gigabits per second.

kIOUSBHostConnectionSpeedSuperPlus

The connected device runs at 10 gigabits per second.

kIOUSBHostConnectionSpeedSuperPlusBy2

The connected device runs at 20 gigabits per second.

kIOUSBHostConnectionSpeedCount

The number of available connection speed values.

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

tIOUSBHostPortStatus

Constants indicating the state of a port.

tIOUSBHostPortType

Constants indicating a port’s type.

