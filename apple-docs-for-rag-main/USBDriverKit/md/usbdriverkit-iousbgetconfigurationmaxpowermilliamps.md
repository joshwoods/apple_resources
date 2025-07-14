

- USBDriverKit
-  IOUSBGetConfigurationMaxPowerMilliAmps 

Function

# IOUSBGetConfigurationMaxPowerMilliAmps

Extracts the maximum bus current a configuration descriptor requires.

DriverKit 19.0+

``` source
uint32_t IOUSBGetConfigurationMaxPowerMilliAmps(uint32_t usbDeviceSpeed, const IOUSBConfigurationDescriptor * descriptor);
```

## Parameters 

`usbDeviceSpeed`  

The operational speed of the device.

`descriptor`  

The configuration descriptor to parse.

## Return Value

The milliamps required.

## Discussion

This method parses a configuration descriptor and returns the number of milliamps required to power the device.

## See Also

### Configuration Descriptors

IOUSBGetNextDescriptor

Gets the next descriptor in a configuration descriptor.

IOUSBGetNextDescriptorWithType

Finds the next descriptor matching a given type within a configuration descriptor.

IOUSBGetNextAssociatedDescriptor

Gets the next descriptor in the specified configuration descriptor that belongs to another container descriptor.

IOUSBGetNextAssociatedDescriptorWithType

Finds the next descriptor matching a specific type within a configuration descriptor that belongs to another container descriptor.

