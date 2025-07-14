

- USBDriverKit
-  IOUSBGetNextDescriptor 

Function

# IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

DriverKit 19.0+

``` source
const IOUSBDescriptorHeader * IOUSBGetNextDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * currentDescriptor);
```

## Parameters 

`configurationDescriptor`  

The configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of `configurationDescriptor`, or `NULL`.

## Return Value

The descriptor pointer, or `NULL` if no descriptor can be returned.

## Discussion

This method advances the current descriptor by its length, and validates that the new descriptor fits within the bounds of the configuration descriptor. Passing `NULL` for the `currentDescriptor` argument returns the first descriptor after the configuration descriptor.

## See Also

### Configuration Descriptors

IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

