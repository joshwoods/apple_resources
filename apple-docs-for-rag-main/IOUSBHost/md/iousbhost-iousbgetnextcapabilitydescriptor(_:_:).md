

- IOUSBHost
-  IOUSBGetNextCapabilityDescriptor(\_:\_:) 

Function

# IOUSBGetNextCapabilityDescriptor(\_:\_:)

Obtains the next device capability descriptor in a BOS descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetNextCapabilityDescriptor(
    _ bosDescriptor: UnsafePointer!,
    _ currentDescriptor: UnsafePointer!
) -> UnsafePointer!
```

## Parameters 

`bosDescriptor`  

A BOS descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `nil`.

## Return Value

A device capability descriptor pointer, or `nil` if no descriptor returns.

## Discussion

This method advances the current descriptor by its length, and validates that the new descriptor fits within the bounds of `bosDescriptor`. Use `nil` for `currentDescriptor` to return the first descriptor after the BOS descriptor.

## See Also

### BOS Descriptor Parsing

func IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityUSB2Extension>!

Obtains the first USB 2.0 extension capability descriptor in a BOS descriptor.

func IOUSBGetNextCapabilityDescriptorWithType(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next descriptor matching a specific type within a BOS descriptor.

func IOUSBGetSuperSpeedDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedUSB>!

Obtains the first SuperSpeed capability descriptor in a BOS descriptor.

func IOUSBGetContainerIDDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityContainerID>!

Obtains the first container ID capability descriptor in a BOS descriptor.

func IOUSBGetBillboardDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityBillboard>!

Obtains the first billboard capability descriptor in a BOS descriptor.

