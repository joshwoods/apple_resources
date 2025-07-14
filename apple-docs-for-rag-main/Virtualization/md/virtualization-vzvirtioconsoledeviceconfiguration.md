

- Virtualization
-  VZVirtioConsoleDeviceConfiguration 

Class

# VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

macOS 13.0+

``` source
class VZVirtioConsoleDeviceConfiguration
```

## Overview

A VZVirtioConsoleDeviceConfiguration object enables serial communication between the guest-operating system and host computer through the Virtio interface. The device sets up one or more ports through VZVirtioConsolePortConfiguration on the Virtio console device.

## Topics

### Creating the configuration object

init()

Creates a console port configuration object.

### Configuring the console ports

var ports: VZVirtioConsolePortConfigurationArray

The list of Virtio port configurations.

## Relationships

### Inherits From

- VZConsoleDeviceConfiguration

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

var consoleDevices: [VZConsoleDeviceConfiguration]

The array of console devices that you expose to the guest operating system.

### Configurations

class VZConsoleDeviceConfiguration

The base class for a console device configuration.

class VZConsolePortConfiguration

The base class for a console port configuration.

class VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

class VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

