

- Virtualization
- VZGenericPlatformConfiguration
-  isNestedVirtualizationEnabled 

Instance Property

# isNestedVirtualizationEnabled

A Boolean value that indicates whether nested virtualization is in an enabled state.

macOS 15.0+

``` source
var isNestedVirtualizationEnabled: Bool { get set }
```

## See Also

### Identifying the platform configuration

var machineIdentifier: VZGenericMachineIdentifier

A value that represents a unique identifier for the virtual machine.

class var isNestedVirtualizationSupported: Bool

A Boolean value that describes whether the platform configuration supports nested virtualization.

class VZGenericMachineIdentifier

An object that represents a unique identifier for a virtual machine.

