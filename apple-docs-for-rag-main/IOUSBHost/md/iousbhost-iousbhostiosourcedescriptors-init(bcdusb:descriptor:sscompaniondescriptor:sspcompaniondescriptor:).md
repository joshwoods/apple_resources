

- IOUSBHost
- IOUSBHostIOSourceDescriptors
-  init(bcdUSB:descriptor:ssCompanionDescriptor:sspCompanionDescriptor:) 

Initializer

# init(bcdUSB:descriptor:ssCompanionDescriptor:sspCompanionDescriptor:)

Creates a new source descriptor structure.

Mac Catalyst 14.0+macOS 10.15+

``` source
init(
    bcdUSB: UInt16,
    descriptor: IOUSBEndpointDescriptor,
    ssCompanionDescriptor: IOUSBSuperSpeedEndpointCompanionDescriptor,
    sspCompanionDescriptor: IOUSBSuperSpeedPlusIsochronousEndpointCompanionDescriptor
)
```

## Parameters 

`bcdUSB`  

The USB version that the device supports, specified as a binary-coded decimal value.

`descriptor`  

A valid endpoint descriptor.

`ssCompanionDescriptor`  

The companion descriptor for SuperSpeed devices.

`sspCompanionDescriptor`  

The companion descriptor for SuperSpeedPlus devices.

## Discussion

The `ssCompanionDescriptor` and `sspCompanionDescriptor` descriptors may be necessary for `bcdUSB` versions `0x0300` and greater, depending on device operating speed and values set in the descriptors. See USB 3.2, 9.5 for more information.

## See Also

### Initializing the Structure

init()

Creates a new source descriptor structure.

