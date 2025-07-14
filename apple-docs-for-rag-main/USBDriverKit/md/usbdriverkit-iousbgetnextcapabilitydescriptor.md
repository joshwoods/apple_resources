

- USBDriverKit
-  IOUSBGetNextCapabilityDescriptor 

Function

# IOUSBGetNextCapabilityDescriptor

Gets the next device capability descriptor in a BOS descriptor.

DriverKit 19.0+

``` source
const IOUSBDeviceCapabilityDescriptorHeader * IOUSBGetNextCapabilityDescriptor(const IOUSBBOSDescriptor * bosDescriptor, const IOUSBDeviceCapabilityDescriptorHeader * currentDescriptor);
```

## Parameters 

`bosDescriptor`  

The BOS descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of the BOS descriptor, or `NULL`.

## Return Value

The device capability descriptor pointer, or `NULL` if no descriptor is available.

## Discussion

This method advances the current descriptor by its length, and validates that the new descriptor fits within the bounds of the BOS descriptor. Passing `NULL` for `currentDescriptor` returns the first descriptor after the BOS descriptor.

## See Also

### BOS Descriptors

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

IOUSBGetPlatformCapabilityDescriptor

Finds the first platform capability descriptor in a BOS descriptor.

IOUSBGetBillboardDescriptor

Finds the first billboard capability descriptor in a BOS descriptor.

