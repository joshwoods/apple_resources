

- IOUSBHost
-  IOUSBGetNextDescriptorWithType(\_:\_:\_:) 

Function

# IOUSBGetNextDescriptorWithType(\_:\_:\_:)

Obtains the next descriptor in a configuration descriptor that matches the type.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBGetNextDescriptorWithType(
    _ configurationDescriptor: UnsafePointer!,
    _ currentDescriptor: UnsafePointer!,
    _ type: UInt8
) -> UnsafePointer!
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `nil`.

`type`  

The descriptor type to find.

## Return Value

A descriptor pointer, or `nil` if no matching descriptor returns.

## Discussion

This method uses IOUSBGetNextDescriptor(_:_:), and further validates that the returned descriptor’s `bDescriptorType` field matches the type parameter.

## See Also

### Configuration Descriptor Parsing

func IOUSBGetNextDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next descriptor in a configuration descriptor.

func IOUSBGetNextAssociatedDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor.

func IOUSBGetNextAssociatedDescriptorWithType(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UnsafePointer&lt;IOUSBDescriptorHeader>!, UInt8) -> UnsafePointer&lt;IOUSBDescriptorHeader>!

Obtains the next associated descriptor in a configuration descriptor and matches the type.

func IOUSBGetNextInterfaceAssociationDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceAssociationDescriptor>!

Obtains the next interface association descriptor in a configuration descriptor.

func IOUSBGetNextInterfaceDescriptor(UnsafePointer&lt;IOUSBConfigurationDescriptor>!, UnsafePointer&lt;IOUSBDescriptorHeader>!) -> UnsafePointer&lt;IOUSBInterfaceDescriptor>!

Obtains the next interface descriptor in a configuration descriptor.

func IOUSBGetConfigurationMaxPowerMilliAmps(UInt32, UnsafePointer&lt;IOUSBConfigurationDescriptor>!) -> UInt32

Obtains the maximum bus current that a configuration descriptor requires.

