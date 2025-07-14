

- Virtualization
-  VZUSBScreenCoordinatePointingDeviceConfiguration 

Class

# VZUSBScreenCoordinatePointingDeviceConfiguration

An object that defines the configuration for a USB pointing device that reports absolute coordinates.

macOS 12.0+

``` source
class VZUSBScreenCoordinatePointingDeviceConfiguration
```

## Overview

A `VZVirtualMachineView` can use this device to send pointer events to the VM.

## Topics

### Creating pointing devices

init()

Creates a new pointing device.

## Relationships

### Inherits From

- VZPointingDeviceConfiguration

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

class VZPointingDeviceConfiguration

The base class for a pointing device configuration.

