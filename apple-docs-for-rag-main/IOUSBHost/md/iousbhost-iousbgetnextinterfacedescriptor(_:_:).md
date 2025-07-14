

- IOUSBHost
-  IOUSBGetNextInterfaceDescriptor(\_:\_:) 

Function

# IOUSBGetNextInterfaceDescriptor(\_:\_:)

Obtains the next interface descriptor in a configuration descriptor.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetNextInterfaceDescriptor(
    _ configurationDescriptor: UnsafePointer!,
    _ currentDescriptor: UnsafePointer!
) -> UnsafePointer!
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `nil`.

## Return Value

The next interface descriptor pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextDescriptorWithType(_:_:_:) to find the next interface descriptor.

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

func IOUSBGetConfigurationMaxPowerMilliAmps(UInt32, UnsafePointer&lt;IOUSBConfigurationDescriptor>!) -> UInt32

Obtains the maximum bus current that a configuration descriptor requires.

