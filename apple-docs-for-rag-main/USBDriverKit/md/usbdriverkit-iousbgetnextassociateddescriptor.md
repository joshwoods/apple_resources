

- USBDriverKit
-  IOUSBGetNextAssociatedDescriptor 

Function

# IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

DriverKit 19.0+

``` source
const IOUSBDescriptorHeader * IOUSBGetNextAssociatedDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * parentDescriptor, const IOUSBDescriptorHeader * currentDescriptor);
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`parentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

## Return Value

A descriptor pointer, or `NULL` if no descriptor can be returned.

## Discussion

This method uses `getNextDescriptor`, but returns `NULL` if it finds another descriptor whose descriptor type field matches the value used for the parent descriptor’s type. Using `NULL` for the current descriptor returns the first descriptor after the parent descriptor.

## See Also

### Configuration Descriptors

IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

