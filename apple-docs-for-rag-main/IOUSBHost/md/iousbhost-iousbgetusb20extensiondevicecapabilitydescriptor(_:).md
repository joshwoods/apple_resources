

- IOUSBHost
-  IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(\_:) 

Function

# IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(\_:)

Obtains the first USB 2.0 extension capability descriptor in a BOS descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetUSB20ExtensionDeviceCapabilityDescriptor(_ bosDescriptor: UnsafePointer!) -> UnsafePointer!
```

## Parameters 

`bosDescriptor`  

A BOS descriptor that contains the descriptors to iterate through.

## Return Value

The device capability extension pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextCapabilityDescriptorWithType(_:_:_:) to find the first device capability extension.

## See Also

### BOS Descriptor Parsing

func IOUSBGetNextCapabilityDescriptorWithType(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next descriptor matching a specific type within a BOS descriptor.

func IOUSBGetNextCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!, UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityDescriptorHeader>!

Obtains the next device capability descriptor in a BOS descriptor.

func IOUSBGetSuperSpeedDeviceCapabilityDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilitySuperSpeedUSB>!

Obtains the first SuperSpeed capability descriptor in a BOS descriptor.

func IOUSBGetContainerIDDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityContainerID>!

Obtains the first container ID capability descriptor in a BOS descriptor.

func IOUSBGetBillboardDescriptor(UnsafePointer&lt;IOUSBBOSDescriptor>!) -> UnsafePointer&lt;IOUSBDeviceCapabilityBillboard>!

Obtains the first billboard capability descriptor in a BOS descriptor.

