

- Virtualization
-  VZGraphicsDisplay 

Class

# VZGraphicsDisplay

A class that represents a graphics display in a VM.

macOS 14.0+

``` source
class VZGraphicsDisplay
```

## Overview

Don’t instantiate a `VZGraphicsDisplay` directly. Graphics displays are first configured on a VZGraphicsDeviceConfiguration subclass. When you create a VZVirtualMachine from the configuration, the displays are available through the displays property of the configuration’s VZGraphicsDevice.

## Topics

### Getting the display size

var sizeInPixels: CGSize

Returns the size of the display, in pixels.

### Observing changes to the display configuration

func addObserver(any VZGraphicsDisplayObserver)

Adds an observer to notify about display configuration changes.

func removeObserver(any VZGraphicsDisplayObserver)

Removes a display configuration change observer.

protocol VZGraphicsDisplayObserver

A protocol you implement to observe state changes in graphic displays.

### Changing the display configuration

func reconfigure(sizeInPixels: CGSize) throws

Resize this display with the new dimensions you provide.

func reconfigure(configuration: VZGraphicsDisplayConfiguration) throws

Reconfigure this display with the new display configuration you provide.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZMacGraphicsDisplay
- VZVirtioGraphicsScanout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZVirtioGraphicsScanoutConfiguration

The configuration for a Virtio graphics device that configures the dimensions of the graphics device for a Linux VM.

### Devices

class VZGraphicsDevice

A class that represents a graphics device in a VM.

class VZMacGraphicsDevice

An object that represents a Mac graphics device.

class VZVirtioGraphicsScanout

A Virtio graphics scanout that corresponds to a Virtio graphics scanout configuration.

class VZMacGraphicsDisplay

An object that represents the graphics display on a Mac.

class VZVirtioGraphicsDevice

A Virtio graphics device.

