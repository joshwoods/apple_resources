

- Virtualization
-  VZGraphicsDevice 

Class

# VZGraphicsDevice

A class that represents a graphics device in a VM.

macOS 14.0+

``` source
class VZGraphicsDevice
```

## Overview

You don’t instantiate a `VZGraphicsDevice` directly. Graphics devices are first configured on the VZVirtualMachineConfiguration through a subclass of VZGraphicsDeviceConfiguration.

When the framework creates a VZVirtualMachine from the configuration, the graphics devices are available through the graphicsDevices property.

The real type of VZGraphicsDevice corresponds to the type used by the configuration.

For example, a VZVirtioGraphicsDeviceConfiguration leads to a device of type VZVirtioGraphicsDevice and a VZMacGraphicsDeviceConfiguration leads to a device of type VZMacGraphicsDevice.

## Topics

### Getting the device’s displays

var displays: [VZGraphicsDisplay]

The list of graphics displays configured for this graphics device.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacGraphicsDevice
- VZVirtioGraphicsDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZMacGraphicsDeviceConfiguration

Configuration for a display attached to a Mac graphics device.

### Devices

class VZGraphicsDisplay

A class that represents a graphics display in a VM.

class VZMacGraphicsDevice

An object that represents a Mac graphics device.

class VZVirtioGraphicsScanout

A Virtio graphics scanout that corresponds to a Virtio graphics scanout configuration.

class VZMacGraphicsDisplay

An object that represents the graphics display on a Mac.

class VZVirtioGraphicsDevice

A Virtio graphics device.

