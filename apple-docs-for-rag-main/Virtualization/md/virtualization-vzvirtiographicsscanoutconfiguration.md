

- Virtualization
-  VZVirtioGraphicsScanoutConfiguration 

Class

# VZVirtioGraphicsScanoutConfiguration

The configuration for a Virtio graphics device that configures the dimensions of the graphics device for a Linux VM.

macOS 13.0+

``` source
class VZVirtioGraphicsScanoutConfiguration
```

## Overview

Use a `VZVirtioGraphicsScanoutConfiguration` to configure the width and height of a Virtio graphics device.

## Topics

### Creating the configuration object

init(widthInPixels: Int, heightInPixels: Int)

Creates a Virtio graphics device with the specified dimensions.

### Instance properties

var heightInPixels: Int

An integer value that describes the height of the graphics device in pixels.

var widthInPixels: Int

An integer value that describes the width of the graphics device in pixels.

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

### Instance properties

var scanouts: [VZVirtioGraphicsScanoutConfiguration]

The array of output devices.

