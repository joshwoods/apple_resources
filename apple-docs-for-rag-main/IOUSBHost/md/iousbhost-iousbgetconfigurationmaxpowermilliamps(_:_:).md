

- IOUSBHost
-  IOUSBGetConfigurationMaxPowerMilliAmps(\_:\_:) 

Function

# IOUSBGetConfigurationMaxPowerMilliAmps(\_:\_:)

Obtains the maximum bus current that a configuration descriptor requires.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetConfigurationMaxPowerMilliAmps(
    _ usbDeviceSpeed: UInt32,
    _ descriptor: UnsafePointer!
) -> UInt32
```

## Parameters 

`usbDeviceSpeed`  

The operational speed of the device.

`descriptor`  

The configuration descriptor to parse.

## Return Value

The number of milliamps necessary.

## Discussion

This method parses a configuration descriptor and returns the number of milliamps necessary to power the device.

## See Also

### Configuration Descriptor Parsing

func IOUSBGetNextDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next descriptor in a configuration descriptor.

func IOUSBGetNextDescriptorWithType(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next descriptor in a configuration descriptor that matches the type.

func IOUSBGetNextAssociatedDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor.

func IOUSBGetNextAssociatedDescriptorWithType(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor and matches the type.

func IOUSBGetNextInterfaceAssociationDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceAssociationDescriptor>!

Obtains the next interface association descriptor in a configuration descriptor.

func IOUSBGetNextInterfaceDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceDescriptor>!

Obtains the next interface descriptor in a configuration descriptor.

