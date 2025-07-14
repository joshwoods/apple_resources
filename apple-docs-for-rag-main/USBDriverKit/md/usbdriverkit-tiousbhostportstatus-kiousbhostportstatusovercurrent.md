

- USBDriverKit
- tIOUSBHostPortStatus
-  kIOUSBHostPortStatusOvercurrent 

Enumeration Case

# kIOUSBHostPortStatusOvercurrent

A port that is in the overcurrent condition.

DriverKit 19.0+

``` source
kIOUSBHostPortStatusOvercurrent
```

## See Also

### Getting the Port Status Flags

kIOUSBHostPortStatusPortTypeMask

A mask for isolating the port bits.

kIOUSBHostPortStatusPortTypePhase

The starting phase for port types.

kIOUSBHostPortStatusPortTypeStandard

A general-purpose USB port.

kIOUSBHostPortStatusPortTypeCaptive

A device that cannot be physically disconnected from the port.

kIOUSBHostPortStatusPortTypeInternal

A device that cannot be physically disconnected from the host machine.

kIOUSBHostPortStatusPortTypeAccessory

A device that might require authentication before drivers can access it.

kIOUSBHostPortStatusPortTypeReserved

A mask for isolating reserved port types.

kIOUSBHostPortStatusConnectedSpeedMask

A mask for isolating the connection state bits.

kIOUSBHostPortStatusConnectedSpeedPhase

The initial phase for connected state bits.

kIOUSBHostPortStatusConnectedSpeedNone

A port with no device connected to it.

kIOUSBHostPortStatusConnectedSpeedFull

A port with a full-speed device connected to it.

kIOUSBHostPortStatusConnectedSpeedLow

A port with a low-speed device connected to it.

kIOUSBHostPortStatusConnectedSpeedHigh

A port with a high-speed device connected to it.

kIOUSBHostPortStatusConnectedSpeedSuper

A port with a super-speed device connected to it.

kIOUSBHostPortStatusConnectedSpeedSuperPlus

A port with a super-speed plus device connected to it.

