

- IOUSBHost
- IOUSBHostIOSourceDescriptors
-  ssCompanionDescriptor 

Instance Property

# ssCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

Mac Catalyst 14.0+macOS 10.15+

``` source
var ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor
```

## Discussion

This descriptor may be necessary for `bcdUSB` versions 0x0300 and greater, depending on device operating speed and values set in the descriptors. See USB 3.2, 9.5 for more information.

## See Also

### Descriptors

var bcdUSB: UInt16

The USB version that the device supports.

var descriptor: IOUSBEndpointDescriptor

The descriptor for a USB endpoint.

var sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

