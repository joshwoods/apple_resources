

- Virtualization
-  VZVirtioGraphicsDeviceConfiguration 

Class

# VZVirtioGraphicsDeviceConfiguration

Configuration that represents the configuration of a Virtio graphics device for a Linux VM.

macOS 13.0+

``` source
class VZVirtioGraphicsDeviceConfiguration
```

## Topics

### Creating the configuration object

init()

Creates a new Virtio graphics device.

### Instance properties

var scanouts: [VZVirtioGraphicsScanoutConfiguration]

The array of output devices.

class VZVirtioGraphicsScanoutConfiguration

The configuration for a Virtio graphics device that configures the dimensions of the graphics device for a Linux VM.

## Relationships

### Inherits From

- VZGraphicsDeviceConfiguration

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

class VZGraphicsDisplayConfiguration

The base class for a graphics display configuration.

class VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

