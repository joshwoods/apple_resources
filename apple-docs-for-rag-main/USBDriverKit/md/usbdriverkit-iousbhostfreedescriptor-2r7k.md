

- USBDriverKit
-  IOUSBHostFreeDescriptor 

Function

# IOUSBHostFreeDescriptor

Releases the specified configuration descriptor.

DriverKit 19.0+

``` source
void IOUSBHostFreeDescriptor(const IOUSBConfigurationDescriptor * descriptor);
```

## Parameters 

`descriptor`  

The descriptor to release.

## See Also

### Disposing of Descriptors

IOUSBHostFreeDescriptor

Releases the specified device descriptor.

IOUSBHostFreeDescriptor

Releases the specified BOS descriptor.

IOUSBHostFreeDescriptor

Releases the specified string descriptor.

