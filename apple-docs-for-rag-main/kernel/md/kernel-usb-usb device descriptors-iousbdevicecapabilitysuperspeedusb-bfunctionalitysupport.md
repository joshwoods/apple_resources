

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilitySuperSpeedUSB
-  bFunctionalitySupport 

Instance Property

# bFunctionalitySupport

The lowest speed at which all the functionality that the device supports is available to the user.

macOS 10.7+

``` source
uint8_t bFunctionalitySupport;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bDevCapabilityType

The capability type.

bmAttributes

A bitmap encoding of supported device-level features.

wSpeedsSupported

The SuperSpeed supported speeds.

bU1DevExitLat

The exit latency of a U1 device.

wU2DevExitLat

The exit latency of a U2 device.

