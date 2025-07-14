

- IOUSBHost
-  IOUSBGetContainerIDDescriptor(\_:) 

Function

# IOUSBGetContainerIDDescriptor(\_:)

Obtains the first container ID capability descriptor in a BOS descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetContainerIDDescriptor(_ bosDescriptor: UnsafePointer!) -> UnsafePointer!
```

## Parameters 

`bosDescriptor`  

A BOS descriptor that contains the descriptors to iterate through.

## Return Value

A container ID capability descriptor pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextCapabilityDescriptorWithType(_:_:_:) to find the first container ID capability descriptor.

## See Also

### BOS Descriptor Parsing

func IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityUSB2Extension>!

Obtains the first USB 2.0 extension capability descriptor in a BOS descriptor.

func IOUSBGetNextCapabilityDescriptorWithType(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next descriptor matching a specific type within a BOS descriptor.

func IOUSBGetNextCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next device capability descriptor in a BOS descriptor.

func IOUSBGetSuperSpeedDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedUSB>!

Obtains the first SuperSpeed capability descriptor in a BOS descriptor.

func IOUSBGetBillboardDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityBillboard>!

Obtains the first billboard capability descriptor in a BOS descriptor.

