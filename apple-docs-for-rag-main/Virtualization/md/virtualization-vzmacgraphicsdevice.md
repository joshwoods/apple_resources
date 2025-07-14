

- Virtualization
-  VZMacGraphicsDevice 

Class

# VZMacGraphicsDevice

An object that represents a Mac graphics device.

macOS 14.0+

``` source
class VZMacGraphicsDevice
```

## Overview

You don’t instantiate a `VZMacGraphicsDevice` directly. Graphics devices are first configured on the VZVirtualMachineConfiguration through a subclass of VZMacGraphicsDeviceConfiguration.  When the framework creates a VZVirtualMachine from the configuration, the graphics devices are available through the `graphicsDevices` property.

## Relationships

### Inherits From

- VZGraphicsDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

### Devices

class VZGraphicsDevice

A class that represents a graphics device in a VM.

class VZGraphicsDisplay

A class that represents a graphics display in a VM.

class VZVirtioGraphicsScanout

A Virtio graphics scanout that corresponds to a Virtio graphics scanout configuration.

class VZMacGraphicsDisplay

An object that represents the graphics display on a Mac.

class VZVirtioGraphicsDevice

A Virtio graphics device.

