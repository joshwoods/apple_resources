

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDeviceCapabilityUSB2Extension 

Type Alias

# IOUSBDeviceCapabilityUSB2Extension

The structure for the USB 2.0 extension device capability.

macOS 10.7+

``` source
typedef struct IOUSBDeviceCapabilityUSB2Extension IOUSBDeviceCapabilityUSB2Extension;
```

## Discussion

See USB 3.2, 9.6.2.1 for more information.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bDevCapabilityType

The capability type.

bmAttributes

A bitmap encoding of supported device-level features.

## See Also

### Capability Descriptors

IOUSBPlatformCapabilityDescriptor

The structure for the platform capability descriptor.

IOUSBPlatformCapabilityDescriptorPtr

A pointer to a USB platform capability descriptor.

IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

IOUSBDeviceCapabilityBillboardAltConfig

The structure for the billboard alternative configuration device capability.

IOUSBDeviceCapabilityBillboardAltConfigCompatibility

The structure for the billboard alternative configuration compatibility device capability.

IOUSBDeviceCapabilityBillboardAltConfigPtr

A pointer to a USB device capability billboard alternative configuration structure.

IOUSBDeviceCapabilityBillboardAltMode

The structure for the billboard alternative mode device capability.

IOUSBDeviceCapabilityBillboardAltModePtr

A pointer to a USB device capability billboard alternative mode structure.

IOUSBDeviceCapabilityBillboardPtr

A pointer to a USB device capability billboard object.

IOUSBDeviceCapabilityContainerID

The structure for the container ID device capability.

IOUSBDeviceCapabilityContainerIDPtr

A pointer to a USB device capability container ID.

IOUSBDeviceCapabilityDescriptorHeader

The device capability descriptor header.

IOUSBDeviceCapabilityDescriptorHeaderPtr

A pointer to a device capability descriptor header.

IOUSBDeviceCapabilitySuperSpeedPlusUSB

The structure for the SuperSpeedPlus USB device capability.

IOUSBDeviceCapabilitySuperSpeedPlusUSBPtr

A pointer to a SuperSpeedPlus USB device capability structure.

IOUSBDeviceCapabilitySuperSpeedUSB

The structure for the SuperSpeed USB device capability.

IOUSBDeviceCapabilitySuperSpeedUSBPtr

A pointer to a SuperSpeed USB device capability structure.

IOUSBDeviceCapabilityUSB2ExtensionPtr

A pointer to a USB 2.0 extension device capability structure.

### Related Documentation

IOUSBDeviceCapabilityUSB2Extension

