

- USBDriverKit
-  IOUSBHostFreeDescriptor 

Function

# IOUSBHostFreeDescriptor

Releases the specified device descriptor.

DriverKit 19.0+

``` source
void IOUSBHostFreeDescriptor(const IOUSBDeviceDescriptor * descriptor);
```

## Parameters 

`descriptor`  

The descriptor to release.

## See Also

### Disposing of Descriptors

IOUSBHostFreeDescriptor

Releases the specified configuration descriptor.

IOUSBHostFreeDescriptor

Releases the specified BOS descriptor.

IOUSBHostFreeDescriptor

Releases the specified string descriptor.

