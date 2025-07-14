

- IOUSBHost
-  IOUSBGetNextCapabilityDescriptorWithType(\_:\_:\_:) 

Function

# IOUSBGetNextCapabilityDescriptorWithType(\_:\_:\_:)

Obtains the next descriptor matching a specific type within a BOS descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetNextCapabilityDescriptorWithType(
    _ bosDescriptor: UnsafePointer!,
    _ currentDescriptor: UnsafePointer!,
    _ type: UInt8
) -> UnsafePointer!
```

## Parameters 

`bosDescriptor`  

A BOS descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `nil`.

`type`  

The descriptor type to find.

## Return Value

A device capability descriptor pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextCapabilityDescriptor(_:_:), and further validates that the returned descriptor’s `bDevCapabilityType` field matches the type parameter.

## See Also

### BOS Descriptor Parsing

func IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityUSB2Extension>!

Obtains the first USB 2.0 extension capability descriptor in a BOS descriptor.

func IOUSBGetNextCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next device capability descriptor in a BOS descriptor.

func IOUSBGetSuperSpeedDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedUSB>!

Obtains the first SuperSpeed capability descriptor in a BOS descriptor.

func IOUSBGetContainerIDDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityContainerID>!

Obtains the first container ID capability descriptor in a BOS descriptor.

func IOUSBGetBillboardDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityBillboard>!

Obtains the first billboard capability descriptor in a BOS descriptor.

