

- Virtualization
-  VZVirtioConsolePortConfiguration 

Class

# VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

macOS 13.0+

``` source
class VZVirtioConsolePortConfiguration
```

## Overview

A console port is a two-way communication channel between a host VZSerialPortAttachment and a VM console port. A Virtio device can have one or more attached console devices. Optionally, you can set a name for a console port and also configure a console port that the guest can use as the system console.

## Topics

### Creating a port configuration

init()

Creates a new Virtio console port configuration.

### Configuring the port

var isConsole: Bool

A Boolean value that indicates whether this port is a console.

var name: String?

The name of the port.

## Relationships

### Inherits From

- VZConsolePortConfiguration

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

class VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

class VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

