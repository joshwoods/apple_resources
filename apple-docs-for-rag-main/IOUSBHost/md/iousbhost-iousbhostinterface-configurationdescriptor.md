

- IOUSBHost
- IOUSBHostInterface
-  configurationDescriptor 

Instance Property

# configurationDescriptor

The configuration descriptor for the interface.

Mac Catalyst 14.0+macOS 10.15+

``` source
var configurationDescriptor: UnsafePointer { get }
```

## Return Value

A pointer to the device’s configuration descriptor.

## See Also

### Retrieving Function Descriptors

var interfaceDescriptor: UnsafePointer&lt;IOUSBInterfaceDescriptor>

The descriptor for the interface.

