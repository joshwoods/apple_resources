

- Virtualization
-  VZMacGraphicsDisplayConfiguration 

Class

# VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

macOS 12.0+

``` source
class VZMacGraphicsDisplayConfiguration
```

## Overview

Use this device to attach a display that’s shown in a VZVirtualMachineView.

## Topics

### Creating the display configuration

convenience init(for: NSScreen, sizeInPoints: NSSize)

Create a display configuration suitable for showing on the specified screen.

init(widthInPixels: Int, heightInPixels: Int, pixelsPerInch: Int)

Create a display configuration with the specified pixel dimensions and pixel density.

### Configuring the display properties

var heightInPixels: Int

The height of the display, in pixels.

var widthInPixels: Int

The width of the display, in pixels.

var pixelsPerInch: Int

The pixel density in pixels per inch.

## Relationships

### Inherits From

- VZGraphicsDisplayConfiguration

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

class VZGraphicsDeviceConfiguration

The base class for a graphics device configuration.

class VZVirtioGraphicsDeviceConfiguration

Configuration that represents the configuration of a Virtio graphics device for a Linux VM.

