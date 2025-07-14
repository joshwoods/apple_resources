

- USBDriverKit
-  IOUSBGetNextInterfaceAssociationDescriptor 

Function

# IOUSBGetNextInterfaceAssociationDescriptor

Finds the next interface association descriptor in a configuration descriptor.

DriverKit 19.0+

``` source
const IOUSBInterfaceAssociationDescriptor * IOUSBGetNextInterfaceAssociationDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * currentDescriptor);
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

## Return Value

An interface association descriptor pointer, or `NULL` if no matching descriptor can be found.

## Discussion

This method uses `getNextDescriptorWithType` to fetch the next interface association descriptor.

## See Also

### Interface Descriptors

IOUSBGetNextInterfaceDescriptor

Finds the next interface descriptor in a configuration descriptor.

