

- Virtualization
-  VZMacOSVirtualMachineStartOptions 

Class

# VZMacOSVirtualMachineStartOptions

A class that describes start options for macOS VMs.

macOS 13.0+

``` source
class VZMacOSVirtualMachineStartOptions
```

## Topics

### Setting recovery mode

var startUpFromMacOSRecovery: Bool

A Boolean value that indicates whether the macOS guest should start in recovery mode.

## Relationships

### Inherits From

- VZVirtualMachineStartOptions

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Platform components

class VZVirtualMachineConfiguration

The environment attributes and list of devices to use during the configuration of macOS or Linux VMs.

class VZMacPlatformConfiguration

The platform configuration for booting macOS on Apple silicon.

class VZPlatformConfiguration

The base class for a platform configuration.

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

class VZMacMachineIdentifier

A unique identifier for a VM.

class VZMacAuxiliaryStorage

An object that contains information the boot loader needs for booting macOS as a guest operating system.

