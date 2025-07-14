

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilityBillboard
-  bAdditionalFailureInfo 

Instance Property

# bAdditionalFailureInfo

A value that indicates additional information on failures.

macOS 10.12+

``` source
uint8_t bAdditionalFailureInfo;
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

bcdVersion

The billboard capability version number.

bReserved

Reserved for future use.

pAltConfigurations

An array of alternative configurations.

