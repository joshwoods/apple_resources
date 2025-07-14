

- Virtualization
-  VZVirtioConsoleDevice 

Class

# VZVirtioConsoleDevice

A class that represents a Virtio console device in a virtual machine.

macOS 13.0+

``` source
class VZVirtioConsoleDevice
```

## Topics

### Configuring the console

var ports: VZVirtioConsolePortArray

The array of console ports that a specific device uses.

var delegate: (any VZVirtioConsoleDeviceDelegate)?

The delegate object for the console device.

protocol VZVirtioConsoleDeviceDelegate

Optional methods that you use to respond when a console port opens or closes in the virtual machine.

## Relationships

### Inherits From

- VZConsoleDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZConsoleDeviceConfiguration

The base class for a console device configuration.

### Devices

class VZConsoleDevice

A class that represents a console device in a VM.

