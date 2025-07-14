

- Virtualization
-  VZGraphicsDisplayConfiguration 

Class

# VZGraphicsDisplayConfiguration

The base class for a graphics display configuration.

macOS 14.0+

``` source
class VZGraphicsDisplayConfiguration
```

## Overview

Don’t instantiate `VZGraphicsDisplayConfiguration` directly. Use one of its subclasses instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacGraphicsDisplayConfiguration
- VZVirtioGraphicsScanoutConfiguration

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

class VZVirtioGraphicsScanoutConfiguration

The configuration for a Virtio graphics device that configures the dimensions of the graphics device for a Linux VM.

### Configurations

class VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZVirtioGraphicsDeviceConfiguration

Configuration that represents the configuration of a Virtio graphics device for a Linux VM.

