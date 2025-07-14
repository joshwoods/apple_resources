

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBDeviceCapabilityBillboard
-  bLength 

Instance Property

# bLength

The size of the descriptor.

macOS 10.12+

``` source
uint8_t bLength;
```

## See Also

### Getting the Properties

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

