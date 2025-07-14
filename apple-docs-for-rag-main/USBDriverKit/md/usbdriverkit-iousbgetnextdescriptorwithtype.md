

- USBDriverKit
-  IOUSBGetNextDescriptorWithType 

Function

# IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

DriverKit 19.0+

``` source
const IOUSBDescriptorHeader * IOUSBGetNextDescriptorWithType(const IOUSBConfigurationDescriptor * configurationDescriptor, const IOUSBDescriptorHeader * currentDescriptor, const uint8_t type);
```

## Parameters 

`configurationDescriptor`  

The configuration descriptor that contains the descriptors to iterate through.

`currentDescriptor`  

A descriptor pointer within the bounds of the configuration descriptor, or `NULL`.

`type`  

The type of descriptor to find.

## Return Value

A descriptor pointer, or `NULL` if no matching descriptor can be found.

## Discussion

This method uses `getNextDescriptor`, and further validates that the returned descriptor’s bDescriptorType field matches the type parameter.

## See Also

### Configuration Descriptors

IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

