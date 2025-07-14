

- USBDriverKit
-  IOUSBGetPlatformCapabilityDescriptor 

Function

# IOUSBGetPlatformCapabilityDescriptor

Finds the first platform capability descriptor in a BOS descriptor.

DriverKit 19.0+

``` source
const IOUSBPlatformCapabilityDescriptor * IOUSBGetPlatformCapabilityDescriptor(const IOUSBBOSDescriptor * bosDescriptor);
```

## Parameters 

`bosDescriptor`  

The BOS descriptor that contains the descriptors to iterate through.

## Return Value

The descriptor pointer, or `NULL` if no matching descriptor can be found.

## Discussion

This method uses `getNextCapabilityDescriptorWithType` to fetch the first `PlatformCapabilityDescriptor.`

## See Also

### BOS Descriptors

IOUSBGetNextCapabilityDescriptor

Gets the next device capability descriptor in a BOS descriptor.

IOUSBGetNextCapabilityDescriptorWithType

Finds the next descriptor matching a given type within a BOS descriptor.

IOUSBGetSuperSpeedDeviceCapabilityDescriptor

Finds the first SuperSpeed device capability descriptor in a BOS descriptor.

IOUSBGetSuperSpeedPlusDeviceCapabilityDescriptor

Finds the first SuperSpeed Plus device capability descriptor in a BOS descriptor.

IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor

Finds the first USB 2.0 extension capability descriptor in a BOS descriptor.

IOUSBGetContainerIDDescriptor

Finds the first Container ID capability descriptor in a BOS descriptor.

IOUSBGetBillboardDescriptor

Finds the first billboard capability descriptor in a BOS descriptor.

