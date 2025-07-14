

- IOUSBHost
- IOUSBHostIOSourceDescriptors
-  sspCompanionDescriptor 

Instance Property

# sspCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

Mac Catalyst 14.0+macOS 10.15+

``` source
var sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor
```

## Discussion

This descriptor may be necessary for `bcdUSB` versions 0x0300 and greater, depending on device operating speed and values set in the descriptors. See USB 3.2, 9.5 for more information.

## See Also

### Descriptors

var bcdUSB: UInt16

The USB version that the device supports.

var descriptor: IOUSBEndpointDescriptor

The descriptor for a USB endpoint.

var ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

