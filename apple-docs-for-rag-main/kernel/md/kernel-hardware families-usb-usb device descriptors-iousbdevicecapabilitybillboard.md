

- Kernel
- Hardware Families
- USB
- USB Device Descriptors
-  IOUSBDeviceCapabilityBillboard 

Type Alias

# IOUSBDeviceCapabilityBillboard

The structure for the billboard device capability.

macOS 10.12+

``` source
typedef struct IOUSBDeviceCapabilityBillboard IOUSBDeviceCapabilityBillboard;
```

## Discussion

For more information about this descriptor type, see USB 3.2, 9.6.2.

## Topics

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bDevCapabilityType

The device capability descriptor type.

iAdditionalInfoURL

The index of a string descriptor providing a URL for detailed information about the product and supported modes.

bNumberOfAlternateModes

The number of alternative supported modes.

bPreferredAlternateMode

The index of the preferred alternative mode.

vCONNPower

The power that the adapter needs for full functionality.

bmConfigured

A value that indicates the state of the alternative modes.

bcdVersion

The billboard capability version number.

bAdditionalFailureInfo

A value that indicates additional information on failures.

bReserved

Reserved for future use.

pAltConfigurations

An array of alternative configurations.

## See Also

### Capability Descriptors

IOUSBPlatformCapabilityDescriptor

The structure for the platform capability descriptor.

IOUSBPlatformCapabilityDescriptorPtr

A pointer to a USB platform capability descriptor.

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

IOUSBDeviceCapabilityUSB2Extension

The structure for the USB 2.0 extension device capability.

IOUSBDeviceCapabilityUSB2ExtensionPtr

A pointer to a USB 2.0 extension device capability structure.

