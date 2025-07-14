

- Virtualization
-  VZUSBControllerConfiguration 

Class

# VZUSBControllerConfiguration

The base class for a USB controller configuration.

macOS 15.0+

``` source
class VZUSBControllerConfiguration
```

## Overview

Don’t create `VZUSBControllerConfiguration` objects directly. Use one of its subclasses, such as VZXHCIControllerConfiguration, instead.

## Topics

### Instance properties

var usbDevices: [any VZUSBDeviceConfiguration]

The list of USB devices.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZXHCIControllerConfiguration

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

class VZXHCIControllerConfiguration

The configuration object for the USB Extensible Host Controller Interface (XHCI) controller.

