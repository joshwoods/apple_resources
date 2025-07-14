

- Virtualization
-  VZGenericPlatformConfiguration 

Class

# VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

macOS 12.0+

``` source
class VZGenericPlatformConfiguration
```

## Topics

### Creating a platform configuration

init()

Returns a new generic platform configuration.

### Identifying the platform configuration

var machineIdentifier: VZGenericMachineIdentifier

A value that represents a unique identifier for the virtual machine.

var isNestedVirtualizationEnabled: Bool

A Boolean value that indicates whether nested virtualization is in an enabled state.

class var isNestedVirtualizationSupported: Bool

A Boolean value that describes whether the platform configuration supports nested virtualization.

class VZGenericMachineIdentifier

An object that represents a unique identifier for a virtual machine.

## Relationships

### Inherits From

- VZPlatformConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

class VZPlatformConfiguration

The base class for a platform configuration.

