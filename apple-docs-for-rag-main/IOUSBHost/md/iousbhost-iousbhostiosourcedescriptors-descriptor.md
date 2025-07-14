

- IOUSBHost
- IOUSBHostIOSourceDescriptors
-  descriptor 

Instance Property

# descriptor

The descriptor for a USB endpoint.

Mac Catalyst 14.0+macOS 10.15+

``` source
var descriptor: IOUSBEndpointDescriptor
```

## Discussion

Initialize this descriptor with a valid IOUSBEndpointDescriptor. See USB 3.2, 9.6.6.

## See Also

### Descriptors

var bcdUSB: UInt16

The USB version that the device supports.

var ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor

The descriptor for a SuperSpeed USB endpoint companion.

var sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor

The descriptor for a SuperSpeedPlus isochronous USB endpoint companion.

