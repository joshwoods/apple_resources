

- Virtualization
- VZGenericPlatformConfiguration
-  machineIdentifier 

Instance Property

# machineIdentifier

A value that represents a unique identifier for the virtual machine.

macOS 13.0+

``` source
@NSCopying
var machineIdentifier: VZGenericMachineIdentifier { get set }
```

## See Also

### Identifying the platform configuration

var isNestedVirtualizationEnabled: Bool

A Boolean value that indicates whether nested virtualization is in an enabled state.

class var isNestedVirtualizationSupported: Bool

A Boolean value that describes whether the platform configuration supports nested virtualization.

class VZGenericMachineIdentifier

An object that represents a unique identifier for a virtual machine.

