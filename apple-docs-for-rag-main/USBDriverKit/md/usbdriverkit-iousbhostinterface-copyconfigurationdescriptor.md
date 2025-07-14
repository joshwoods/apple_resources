

- USBDriverKit
- IOUSBHostInterface
-  CopyConfigurationDescriptor 

Instance Method

# CopyConfigurationDescriptor

Retrieves the parent configuration descriptor for this interface.

DriverKit 19.0+

``` source
const IOUSBConfigurationDescriptor * CopyConfigurationDescriptor();
```

## Return Value

The configuration descriptor for this interface. It’s your responsibility to free the returned descriptor.

## See Also

### Getting Interface-Related Descriptors

GetInterfaceDescriptor

Returns the version of the interface descriptor that is associated with the specified configuration.

CopyStringDescriptor

Returns a descriptor from the device in the specified language.

CopyStringDescriptor

Returns a string descriptor from the device.

