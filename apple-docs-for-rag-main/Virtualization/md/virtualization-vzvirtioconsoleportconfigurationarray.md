

- Virtualization
-  VZVirtioConsolePortConfigurationArray 

Class

# VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

macOS 13.0+

``` source
class VZVirtioConsolePortConfigurationArray
```

## Overview

This array stores a collection of port configurations for a VZVirtioConsoleDeviceConfiguration. The index in the array corresponds to the port index that the VM uses. You can set a maximumPortCount value, but the value must be larger than the highest indexed port. If there’s no `maximumPortCount` value set, the framework uses the value the highest indexed port.

## Topics

### Determining the number of ports

var maximumPortCount: UInt32

An unsigned integer that represents the maximum number of ports allocated by this device.

### Accessing a specific port

subscript(Int) -> VZVirtioConsolePortConfiguration?

Returns the Virtio console port configuration as the specified index.

## Relationships

### Inherits From

- NSObject

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

class VZConsoleDeviceConfiguration

The base class for a console device configuration.

class VZConsolePortConfiguration

The base class for a console port configuration.

class VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

class VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

