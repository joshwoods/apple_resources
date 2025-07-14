

- USBDriverKit
-  IOUSBGetNextAssociatedDescriptorWithType 

Function

# IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

DriverKit 19.0+

``` source
const IOUSBDescriptorHeader * IOUSBGetNextAssociatedDescriptorWithType(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * parentDescriptor, const IOUSBDescriptorHeader * currentDescriptor, const uint8_t type);
```

## Parameters 

`configurationDescriptor`  

A configuration descriptor that contains the descriptors to iterate through.

`parentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

`type`  

The descriptor type to find.

## Return Value

A descriptor pointer, or `NULL` if no matching descriptor is found.

## Discussion

This method uses `getNextAssociatedDescriptor`, and further validates that the returned descriptor’s type field matches the type parameter passed to this method.

## See Also

### Configuration Descriptors

IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

