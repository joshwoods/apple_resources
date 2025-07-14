

- Virtualization
-  VZMacTrackpadConfiguration 

Class

# VZMacTrackpadConfiguration

The class that represents the configuration for a Mac trackpad.

macOS 13.0+

``` source
class VZMacTrackpadConfiguration
```

## Overview

Note

The framework recognizes this device in virtual machines running macOS 13 and later. To support both macOS 13.0 and earlier guests, set pointingDevices to an array that contains both a VZMacTrackpadConfiguration and a VZUSBScreenCoordinatePointingDeviceConfiguration object.

The VZVirtualMachineView uses this device to send pointer events and multi-touch trackpad gestures to the virtual machine. In macOS 13 and later, guests use the multi-touch trackpad device, while earlier versions of macOS uses the USB pointing device.

## Topics

### Initializers

init()

Creates a new Mac trackpad configuration.

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

class VZUSBScreenCoordinatePointingDeviceConfiguration

An object that defines the configuration for a USB pointing device that reports absolute coordinates.

class VZPointingDeviceConfiguration

The base class for a pointing device configuration.

