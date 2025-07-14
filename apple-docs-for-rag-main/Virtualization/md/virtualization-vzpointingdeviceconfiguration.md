

- Virtualization
-  VZPointingDeviceConfiguration 

Class

# VZPointingDeviceConfiguration

The base class for a pointing device configuration.

macOS 12.0+

``` source
class VZPointingDeviceConfiguration
```

## Overview

Don’t instantiate a `VZPointingDeviceConfiguration` directly, use one of its subclasses like VZUSBScreenCoordinatePointingDeviceConfiguration instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacTrackpadConfiguration
- VZUSBScreenCoordinatePointingDeviceConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Pointing devices

class VZMacTrackpadConfiguration

The class that represents the configuration for a Mac trackpad.

class VZUSBScreenCoordinatePointingDeviceConfiguration

An object that defines the configuration for a USB pointing device that reports absolute coordinates.

