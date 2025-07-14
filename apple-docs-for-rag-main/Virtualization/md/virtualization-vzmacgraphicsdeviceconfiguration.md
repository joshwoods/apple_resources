

- Virtualization
-  VZMacGraphicsDeviceConfiguration 

Class

# VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

macOS 12.0+

``` source
class VZMacGraphicsDeviceConfiguration
```

## Overview

Use this device to attach a display that’s shown in a VZVirtualMachineView.

## Topics

### Creating the graphics device configuration

init()

Creates a new Mac graphics device configuration.

### Configuring displays

var displays: [VZMacGraphicsDisplayConfiguration]

The displays associated with this graphics device.

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

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZVirtioGraphicsDeviceConfiguration

Configuration that represents the configuration of a Virtio graphics device for a Linux VM.

