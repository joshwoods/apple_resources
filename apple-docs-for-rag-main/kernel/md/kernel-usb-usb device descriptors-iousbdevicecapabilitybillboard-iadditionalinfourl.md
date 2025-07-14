

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilityBillboard
-  iAdditionalInfoURL 

Instance Property

# iAdditionalInfoURL

The index of a string descriptor providing a URL for detailed information about the product and supported modes.

macOS 10.12+

``` source
uint8_t iAdditionalInfoURL;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bDevCapabilityType

The device capability descriptor type.

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

