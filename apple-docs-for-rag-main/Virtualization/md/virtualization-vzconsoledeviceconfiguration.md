

- Virtualization
-  VZConsoleDeviceConfiguration 

Class

# VZConsoleDeviceConfiguration

The base class for a console device configuration.

macOS 13.0+

``` source
class VZConsoleDeviceConfiguration
```

## Overview

Don’t instantiate VZConsoleDeviceConfiguration directly, instead use one of its subclasses like VZVirtioConsoleDeviceConfiguration instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioConsoleDeviceConfiguration

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

class VZConsolePortConfiguration

The base class for a console port configuration.

class VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

class VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

class VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

