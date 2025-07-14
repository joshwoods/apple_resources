

- Virtualization
-  VZConsolePortConfiguration 

Class

# VZConsolePortConfiguration

The base class for a console port configuration.

macOS 13.0+

``` source
class VZConsolePortConfiguration
```

## Overview

Don’t instantiate `VZConsolePortConfiguration` directly, instead use one of its subclasses like VZVirtioConsolePortConfiguration.

## Topics

### Configuring the attachment

var attachment: VZSerialPortAttachment?

The serial port attachment.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioConsolePortConfiguration

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

class VZVirtioConsoleDeviceConfiguration

A console device that enables communication between the host and the guest using console ports through a Virtio interface.

class VZVirtioConsolePortConfiguration

A class that represents the configuration options you can set on a Virtio console port.

class VZVirtioConsolePortConfigurationArray

A class that represents a collection of Virtio console port configurations.

