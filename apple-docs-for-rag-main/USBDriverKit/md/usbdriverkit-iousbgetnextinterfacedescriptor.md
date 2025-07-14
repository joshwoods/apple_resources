

- USBDriverKit
-  IOUSBGetNextInterfaceDescriptor 

Function

# IOUSBGetNextInterfaceDescriptor

Finds the next interface descriptor in a configuration descriptor.

DriverKit 19.0+

``` source
const IOUSBInterfaceDescriptor * IOUSBGetNextInterfaceDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * currentDescriptor);
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

## Return Value

An interface description pointer, or `NULL` if no matching descriptor is found.

## Discussion

This method uses `getNextDescriptorWithType` to fetch the next interface descriptor.

## See Also

### Interface Descriptors

IOUSBGetNextInterfaceAssociationDescriptor

Finds the next interface association descriptor in a configuration descriptor.

