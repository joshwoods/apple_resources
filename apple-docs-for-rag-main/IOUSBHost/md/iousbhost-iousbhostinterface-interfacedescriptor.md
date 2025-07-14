

- IOUSBHost
- IOUSBHostInterface
-  interfaceDescriptor 

Instance Property

# interfaceDescriptor

The descriptor for the interface.

Mac Catalyst 14.0+macOS 10.15+

``` source
var interfaceDescriptor: UnsafePointer { get }
```

## Return Value

A pointer to the interface’s descriptor.

## See Also

### Retrieving Function Descriptors

var configurationDescriptor: UnsafePointer&lt;IOUSBConfigurationDescriptor>

The configuration descriptor for the interface.

