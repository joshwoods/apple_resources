

- Virtualization
-  VZMacOSConfigurationRequirements 

Class

# VZMacOSConfigurationRequirements

An object that describes the parameter constraints required by a specific configuration of macOS.

macOS 12.0+

``` source
class VZMacOSConfigurationRequirements
```

## Topics

### Configuration Requirements

var hardwareModel: VZMacHardwareModel

The hardware model for this configuration.

var minimumSupportedCPUCount: Int

The minimum supported number of CPUs for this configuration.

var minimumSupportedMemorySize: UInt64

The minimum supported memory size for this configuration.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacHardwareModel

A specification for the hardware elements and configurations present in a particular Mac hardware model.

### Installers

class VZMacOSInstaller

An object you use to install macOS on the specified virtual machine.

class VZMacOSRestoreImage

An object that describes a version of macOS to install on to a virtual machine.

