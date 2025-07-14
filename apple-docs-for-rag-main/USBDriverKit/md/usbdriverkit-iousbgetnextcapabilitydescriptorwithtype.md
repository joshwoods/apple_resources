

- USBDriverKit
-  IOUSBGetNextCapabilityDescriptorWithType 

Function

# IOUSBGetNextCapabilityDescriptorWithType

Finds the next descriptor matching a given type within a BOS descriptor.

DriverKit 19.0+

``` source
const IOUSBDeviceCapabilityDescriptorHeader * IOUSBGetNextCapabilityDescriptorWithType(const IOUSBBOSDescriptor * bosDescriptor, const IOUSBDeviceCapabilityDescriptorHeader * currentDescriptor, const uint8_t type);
```

## Parameters 

`bosDescriptor`  

The BOS descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of the BOS descriptor, or `NULL`.

`type`  

The descriptor type to find.

## Return Value

A descriptor pointer, or `NULL` if no matching descriptor is available.

## Discussion

This method uses `getNextCapabilityDescriptor`, and further validates that the returned descriptor’s `bDevCapabilityType` field matches the type parameter.

## See Also

### BOS Descriptors

IOUSBGetNextCapabilityDescriptor

Gets the next device capability descriptor in a BOS descriptor.

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

