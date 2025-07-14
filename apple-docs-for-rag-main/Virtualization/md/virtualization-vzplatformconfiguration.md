

- Virtualization
-  VZPlatformConfiguration 

Class

# VZPlatformConfiguration

The base class for a platform configuration.

macOS 12.0+

``` source
class VZPlatformConfiguration
```

## Overview

Don’t instantiate directly `VZPlatformConfiguration`, use one of its subclasses, such as VZGenericPlatformConfiguration or VZMacPlatformConfiguration instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZGenericPlatformConfiguration
- VZMacPlatformConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

### Configurations

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZVirtualMachineStartOptions

The abstract class for VM start options.

class VZGenericPlatformConfiguration

The platform configuration for a generic Intel or ARM virtual machine.

