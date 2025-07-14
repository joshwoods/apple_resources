

- Virtualization
-  VZConsoleDevice 

Class

# VZConsoleDevice

A class that represents a console device in a VM.

macOS 13.0+

``` source
class VZConsoleDevice
```

## Overview

Don’t instantiate a `VZConsoleDevice` directly: You first configure console devices on the VZVirtualMachineConfiguration through a subclass of VZConsoleDeviceConfiguration. After you create VZVirtualMachine from the configuration, the console devices are available through the consoleDevices property.

The actual type of `VZConsoleDevice` corresponds to the type that the configuration uses. For example, a VZVirtioConsoleDeviceConfiguration is a device of type VZVirtioConsoleDevice.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioConsoleDevice

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

class VZVirtioConsoleDevice

A class that represents a Virtio console device in a virtual machine.

