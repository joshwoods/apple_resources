

- Virtualization
- VZMacHardwareModel
-  isSupported 

Instance Property

# isSupported

A Boolean value that indicates whether the host supports this hardware model.

macOS 12.0+

``` source
var isSupported: Bool { get }
```

## Discussion

If this hardware model isn’t supported by the host, the VZVirtualMachineConfiguration won’t validate.

The validation error of the `VZVirtualMachineConfiguration` provides more information about why the hardware model isn’t supported.

## See Also

### Configuring the hardware model

var dataRepresentation: Data

Returns the opaque data representation of the hardware model.

