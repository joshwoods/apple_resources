

- USBDriverKit
- IOUSBHostInterface
-  GetInterfaceDescriptor 

Instance Method

# GetInterfaceDescriptor

Returns the version of the interface descriptor that is associated with the specified configuration.

DriverKit 19.0+

``` source
const IOUSBInterfaceDescriptor * GetInterfaceDescriptor(const IOUSBConfigurationDescriptor * configurationDescriptor);
```

## Parameters 

`configurationDescriptor`  

The configuration descriptor that owns the interface.

## Return Value

The interface descriptor structure.

## See Also

### Getting Interface-Related Descriptors

CopyConfigurationDescriptor

Retrieves the parent configuration descriptor for this interface.

CopyStringDescriptor

Returns a descriptor from the device in the specified language.

CopyStringDescriptor

Returns a string descriptor from the device.

