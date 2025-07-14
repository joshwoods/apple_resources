

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilitySuperSpeedUSB
-  bmAttributes 

Instance Property

# bmAttributes

A bitmap encoding of supported device-level features.

macOS 10.7+

``` source
uint8_t bmAttributes;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bDevCapabilityType

The capability type.

wSpeedsSupported

The SuperSpeed supported speeds.

bFunctionalitySupport

The lowest speed at which all the functionality that the device supports is available to the user.

bU1DevExitLat

The exit latency of a U1 device.

wU2DevExitLat

The exit latency of a U2 device.

