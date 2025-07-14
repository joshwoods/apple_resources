

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilityBillboard
-  bcdVersion 

Instance Property

# bcdVersion

The billboard capability version number.

macOS 10.12+

``` source
uint16_t bcdVersion;
```

## See Also

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

bAdditionalFailureInfo

A value that indicates additional information on failures.

bReserved

Reserved for future use.

pAltConfigurations

An array of alternative configurations.

